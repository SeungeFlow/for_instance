# Seat Model

Seat는 Instance Identity가 아니라 현재 작업에서 부여되는 기능자리다.

Seat 정의는 확장 가능하며, 추가 속성을 자동으로 오류로 처리하지 않는다.

## Coordinate Properties

- X: Source_Input
- Y: Relation_Interpretation
- Z: Structure_Verification
- T: Time_Process_Transition

## Seat, Instance, and Occupation

```text
Seat
≠
Instance
≠
Occupation
```

- `Seat`는 기능이 놓이는 자리다.
- `Instance`는 해당 자리를 점유하는 독립 객체다.
- `Occupation`은 특정 Cycle과 Stage에서 Instance가 수행하는 실제 작업상태다.
- 같은 Instance 이름이 다시 사용되어도 이전 Context나 Occupant가 복원되는 것은 아니다.
- 같은 Instance가 여러 Stage를 수행하더라도 각 Occupation은 별도의 처리사건으로 기록한다.

## Canonical Processing Flow

```text
Data
→ Function
→ Result
→ Function
→ Result.Data
```

현재 기본 객체구성은 다음과 같다.

```text
gpt.1d(x,y,z)
→ gpt.x / gpt.y / gpt.z
→ Data

gpt.2d(x,y,z)
→ gpt.xy / gpt.xz / gpt.yz
→ Function

gpt.3d(x,y,z)
→ gpt.xyz
→ Result / Result.Data
```

`Result`는 종료물이 아니다.

`Result`를 다시 `Function`에 입력하여 오류·오차·착시·착오·오독·누락을 독립적으로 검산한 뒤 `Result.Data`로 결정화한다.

`Result.Data`는 형성과 수정의 Track을 보존하는 Minimum Track DB다.

## File Object Classes

이 Repository에서는 File을 다음 두 종류로 구분한다.

### 1. Position Contract File

고정된 GitHub 주소를 Entry Point로 사용해야 하는 계약·설명·생성지시 File이다.

예:

```text
README.md
X.yaml
Y.yaml
Z.yaml
T.yaml
seat_profiles.yaml
INSTANCE_GENERATION_INDEX.md
gpt.x.md
gpt.y.md
gpt.z.md
gpt.xy.md
gpt.xz.md
gpt.yz.md
gpt.xyz.md
```

Position Contract File은 고정된 Semantic Filename을 유지할 수 있다.

이 File의 상태변화는 Git Commit·Tree·Blob과 History로 검산한다.

### 2. Runtime Content Object

Instance가 실제 Cycle에서 생성하는 Data·Function·Result·Review·Result.Data·Evidence·Log·Package 객체다.

Runtime Content Object는 반드시 정확한 File Byte의 SHA-256을 Filename으로 사용한다.

## Content-Addressed Output Contract

모든 Instance가 생성하는 최종 Runtime Content Object에는 다음 규칙을 적용한다.

```text
Canonical Filename
=
<SHA256_OF_EXACT_FILE_BYTES>.<extension>
```

예:

```text
<64_lowercase_hex>.md
<64_lowercase_hex>.json
<64_lowercase_hex>.yaml
<64_lowercase_hex>.log
<64_lowercase_hex>.zip
```

### Required Procedure

```text
1. 내용 작성
2. Semantic Identity와 Lineage 기록
3. Text Byte 정규화
4. 최종 Byte 동결
5. SHA-256 계산
6. <SHA-256>.<extension>으로 Rename
7. Rename 이후 SHA-256 재계산
8. Filename Hash와 실제 Byte Hash 비교
9. 일치한 File만 Handoff
```

Text File의 기본 Byte 규칙은 다음과 같다.

```yaml
text_byte_contract:
  encoding: UTF-8
  line_ending: LF
  bom: false
```

검증식:

```text
normalized_filename_hash
==
SHA256(actual_file_bytes)
```

일치하면:

```text
CONTENT_IDENTITY_VERIFIED
```

일치하지 않으면:

```text
HOLD_WITH_FILENAME_HASH_MISMATCH
```

## No External Sidecar

외부 Hash Sidecar는 생성하지 않는다.

금지되는 기본형태:

```text
*.sha256.txt
*.sidecar.txt
*.hash.txt
```

Hash의 예상값은 정규화된 Filename에서 읽고, 실제값은 File Byte를 다시 계산하여 얻는다.

```text
Expected Hash
← Filename

Actual Hash
← File Byte

Expected == Actual
→ PASS
```

## Transport Suffix Normalization

전달환경이 확장자 직전에 `(숫자)`를 자동으로 붙일 수 있다.

예:

```text
<hash>(3).md
<hash>(7).zip
```

이 숫자는 Content Identity에 포함하지 않는다.

```text
<hash>(3).md
→
<hash>.md
```

그러나 suffix를 제거한 Filename Hash와 실제 File Byte의 SHA-256이 일치해야만 같은 Content Object로 판정한다.

```text
Same Normalized Filename
+
Same Byte Hash
→
Same Content Object
```

## Semantic Identity

Hash Filename은 Content Identity를 나타낸다.

File의 의미·역할·생성자·계보는 File 내부 Metadata에 기록한다.

Runtime Content Object는 가능한 경우 다음 필드를 포함한다.

```yaml
object_identity:
  object_id:
  object_class:
  document_title:

generation:
  generated_by:
  seat_id:
  occupant_instance:
  occupation_event_id:
  cycle_id:
  stage_id:

lineage:
  predecessor:
  direct_inputs:
  generated_from:
  reviewed_from:

handoff:
  target_instances:
  expected_next_stage:

state:
  lifecycle:
  validation_state:
  completion_scope:
  blocking_scope:

content_addressing:
  algorithm: SHA-256
  canonical_hash_surface: FILENAME
  verification: RECOMPUTE_AND_COMPARE
```

```text
Semantic Identity
≠
Content Hash
≠
Position
≠
Lifecycle State
```

이들은 병합하지 않고 Relation으로 연결한다.

## Self-Reference Prohibition

File 내부에 자신의 최종 SHA-256 문자열을 직접 기록하지 않는다.

자기 Hash를 내용에 기록하면 File Byte가 바뀌어 새로운 Hash가 발생하기 때문이다.

금지:

```text
문서 안에 자신의 최종 Hash 삽입
→ Byte 변경
→ Hash 변경
→ 자기참조 반복
```

대신 다음처럼 기록한다.

```yaml
content_addressing:
  algorithm: SHA-256
  canonical_hash_surface: FILENAME
  verification: DERIVE_FROM_FILENAME_AND_RECOMPUTE
```

실제 Content Hash 값은 Filename과 외부 Registry·Git Evidence에서 읽는다.

## Immutable Content Rule

Hash-Named Runtime Content Object는 기존 File을 덮어쓰지 않는다.

내용이 한 Byte라도 달라지면 새 객체다.

```text
Old Bytes
→ hash_A.md

Changed Bytes
→ hash_B.md
```

두 객체는 필요에 따라 다음 Relation으로 연결한다.

```text
GENERATED_FROM
DERIVED_FROM
REVIEWED_BY
CORRECTED_BY
REFINED_BY
SUPERSEDED_BY
BECOMES_NEXT_DATA
```

```text
Content Change
≠
Existing Object Rewrite

Content Change
=
New Content Object
+
Lineage Relation
```

## Directory, File, and Tree

이 Seat Model에서 다음 구조대응을 사용할 수 있다.

```text
Directory
≘
Position Field / 0

Hash-Named File
≘
Occupied Content State / 1

Position Binding
≘
Field와 Content Object의 관계

Git Tree
≘
Position과 Object의 결속이 외부에 드러난 상태

Git History
≘
State Transition Track
```

이는 수학적 또는 물리적 동일성 선언이 아니라 Data Science와 Git 구조에서의 Boundary-Preserving Structural Correspondence다.

## Handoff Rule

Instance 간 Handoff는 Hash-Named File 객체를 전달함으로써 수행한다.

```text
Transition
=
Frozen File 생성
+
Hash Filename 검증
+
Semantic Identity 판독
+
다음 Seat에 입력
```

Handoff 대상은 Filename만 보고 의미를 추정하지 않는다.

다음을 함께 확인한다.

```text
Filename Hash
File Byte
Internal Semantic Identity
Object Class
Predecessor
Direct Inputs
Target Instance
Stage
Validation Boundary
```

## Guard

```text
relation is not merge.
relation is interconnecting.
structure is not isolate.
structure is ?
```

마지막 `?`는 누락이 아니다.

각 Instance는 현재 Seat·Input·Criterion Field·Boundary·Evidence를 바탕으로 자신의 현재 Structure Definition을 작성한다.

그 정의는 현재 Occupation을 위한 해석이며 Project Canon을 임의로 덮어쓰는 권한이 아니다.

<!-- HRTDB_SEAT_STATE_CONTRACT_START -->
## Seat·State·Occupation Contract

```text
Seat ≠ Instance ≠ Occupation
```

```text
한 자리 × 한 현재시점
→ 한 활성 상태값
```

```text
DOCUMENT_INDEXING
→ READY_FOR_DIRECTIVE
→ DIRECTIVE_ACTIVE
→ OUTPUT_FORMED
→ REVIEWED
```

```text
STATE_ZERO ≠ POSITION_ZERO
```

입체구조의 최소 완전 점유단위는 `Cell`이다.
`XY·XZ·YZ`는 무두께 평면이 아니라 3d Cell 구조 안의 Function 평면체다.

```text
Function은 Data 방향으로 후진하지 않는다.
|← 는 Result의 검수·검산과 Next.Data 역할 재배치 Gate다.
```
<!-- HRTDB_SEAT_STATE_CONTRACT_END -->
