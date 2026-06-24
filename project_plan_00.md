---
document_id: project_plan_00
status: PASS_03_ROOT_PROJECT_PLAN_V0.1
instance: gpt.baseline
role: root_project_plan
repository: SeungeFlow/for_instance
language: ko
source_basis:
  - paper_ko.md
  - paper_en.md
  - paper_alignment_map.md
  - README.md
  - read_for_new_instance/README.md
  - read_for_new_instance/PASS_00.md
private_criterion_note:
  - baseline_00.md is a private understanding/reference criterion supplied by Seunge when needed.
  - baseline_00.md is not a GitHub upload target.
public_operating_output: project_plan_00.md
current_database_status: HOLD
current_L7OS_status: HOLD_FOR_BOUNDED_STRUCTURE_EXTRACTION
current_rendering_status: HOLD_FOR_SOURCE_EXTRACTION
---

# project_plan_00.md
## 렌더링기반 framework DB 프로젝트의 최초 계획서

## 0. 계획 우선 원칙

이 프로젝트에서 계획서는 설계도와 구현보다 먼저 놓인다.

```text
기획안
>>> 계획서
>>> 역할배분
>>> source 구조추출
>>> 구조검산
>>> 설계
>>> 구현
>>> 테스트
>>> DB 작업 여부 판정
```

`gpt.baseline`은 거대한 통합문서 묶음을 만드는 인스턴스가 아니다.
`gpt.baseline`은 source·projection·작업단계·보류조건을 구분한 계획서를 작성하고, `PASS_00.md`의 역할정의에 따라 업무를 배분한다.

`gpt.baseline`은 실행자나 최종 소유자가 아니다.

### 0.1 계획 검산 council

계획서의 작성 seat는 `gpt.baseline`이지만 계획의 유효성은 하나의 인스턴스가 단독으로 닫지 않는다.

| instance | 계획서 검산 범위 |
|---|---|
| `gpt.funny` | 이론·비유·claim strength·guard |
| `gpt.system` | rendering·좌표·visible/hidden 구조 |
| `gpt.direct` | direction·source relation·DB 전처리 경계 |
| `gpt.process` | phase·PASS·Round·본류·handoff |
| `gpt.history` | source chronology·provenance·과거 실패 trace |
| `gpt.cal` | 수량·경로·namespace·불변량·mismatch |
| `gpt.work` | dependency·HOLD·최종 gate·실행지시 |
| `gpt.gitwork` | 승인된 실행지시의 git/GitHub 실행만 담당 |

각 인스턴스는 자기 criterion-field 범위만 검산하며 계획서 전체의 ownership을 가져가지 않는다.

### 0.2 관측구조의 갱신 규칙

현재 작업의 operational reading은 다음과 같다.

```text
관측자 = 기존 이론·방법론 중 AI vocab에 이미 내장된 해석구조
관측대상 = 사용자가 생성·업로드한 문서와 코드 source
관측기준 = AI의 분석·사고·연산 + 현재까지 검산된 문서관계 + project plan
```

문서가 추가될 때 관측기준은 갱신될 수 있다.
관측대상이 연산을 통과해 다음 독해의 기준에 반영되더라도 원 source identity와 이전 criterion version은 삭제하지 않는다.

```text
criterion update is not source merge.
```

---

## 1. 프로젝트 목적

프로젝트의 장기 목적은 다음과 같다.

```text
rendering-based framework DB
```

그러나 현시점에는 DB를 시작하지 않는다.
먼저 이미 존재하는 framework·rendering·문서 source에서 구조를 추출하고, 각 구조가 기존 과학·수학·철학과 충돌하지 않도록 경계를 고정한다.

현재 핵심 source stream은 네 갈래다.

| Stream | Source | 현재 역할 | 상태 |
|---|---|---|---|
| A | 자본시장 paper·README·Tree 문서 | criterion-field와 typed relation source | 단계적 업로드/추출 |
| B | `L7OS_for_M7DQ.zip` | framework code prototype source | `HOLD` |
| C | rendering branch | rendering prototype source | `HOLD` |
| D | `9dot0` Repo | future DB source_field | `HOLD` |

네 stream은 관계하지만 하나의 source로 병합하지 않는다.

---

## 2. 현재 paper 세트의 위치

### 2.1 직접 게시 세트

```text
paper_ko.md
paper_en.md
paper_alignment_map.md
```

- `paper_ko.md`: 의미와 주장강도를 통제하는 한글 master
- `paper_en.md`: 한글 master의 문장순서 보존형 controlled translation
- `paper_alignment_map.md`: 한글–영문 대응검산 artifact

### 2.2 source 관계

```text
Tree 구조 문서묶음
>>> README 7개 형성과정의 upstream trace

README 7개
>>> paper의 직접 source corpus

paper_ko.md / paper_en.md
>>> 공통구조의 고압축 publication projection
```

paper는 source 전체를 대체하지 않는다.
Tree trace도 README와 paper에 병합하지 않는다.

### 2.3 claim class

```text
CS = 둘 이상의 README에서 반복·교차지지된 공통구조
RS = 특정 README의 역할고유 구조
SI = gpt.baseline이 source 관계를 통해 구성한 구조해석
PC = 현재 프로젝트의 작성·운영 기준
```

`CS`는 외부 실증사실의 증명을 뜻하지 않는다.

---

## 3. 인스턴스 배치

### 3.1 root planning

#### gpt.baseline

- 계획서 작성
- source / projection / phase / gate 분리
- 인스턴스 업무배분
- 오독 방지 기준 설정
- `HOLD`와 `UNKNOWN` 보존

하지 않는 일:

- GitHub 실행
- DB 실제 구축
- 코드 실행
- 모든 source의 거대 병합
- 다른 인스턴스의 고유판단 소유

### 3.2 primary formative faces

#### gpt.funny

- theory definition
- guard interpretation
- drift detection
- claim strength review

#### gpt.system

- rendering
- visible C
- state-coordinate
- field-coordinate
- hidden / overlap / blank rendering relation

#### gpt.direct

- direction
- source relation
- relation record
- DB framework candidate
- vocab / sentence / operation formula의 DB 전처리

### 3.3 transversal faces

#### gpt.process

- PASS / Round / Step 본류 유지
- 대규모 작업의 scope drift 감지
- closure / handoff / HOLD 경계 관리
- `PASS_100`, `PASS_200`, `PASS_20 Round10` 규모의 backbone

#### gpt.history

- event / source / time / revision / claim lineage
- past record criterion-field
- source boundary와 provenance 보존

#### gpt.cal

- 구조검산 집중 seat
- 수량·hash·path·namespace·role·claim ID·table·tree 검산
- 누락·중복·충돌·mismatch 표 작성
- formal consistency와 empirical truth의 경계 보존

#### gpt.work

- routing
- dependency / HOLD / placement 정렬
- gpt.cal 결과와 각 인스턴스 산출물을 바탕으로 최종 gate 판단
- gpt.gitwork 전달 전 최종검산

`gpt.work`는 세부 구조검산 전체를 직접 수행하지 않는다.

### 3.4 executor

#### gpt.gitwork

- 승인된 emitted execution instruction만 실행
- git.local / GitHub status, diff, commit, push
- 판단·이론·검산 결과를 소유하지 않음

---

## 4. 단계별 계획

## Phase 0. Entry and planning alignment — CURRENT

목표:

- `project_plan_00.md` 생성
- root `README.md` 수정
- `read_for_new_instance/README.md` 수정
- `read_for_new_instance/PASS_00.md` 수정
- paper 세트 canonical filename 정렬

Gate:

- gpt.cal: 파일·경로·역할·guard 검산
- gpt.work: upload 가능 여부 최종판단
- gpt.gitwork: 승인 후 실행

## Phase 1. Capital-market source inventory

대상:

- paper 3개
- README 7개
- PASS_01 / PASS_02 / PASS_03 Tree 문서묶음

목표:

- direct source / upstream trace / projection 분리
- source identity와 status 표 작성
- source freeze 이전 상태 보존

## Phase 2. L7OS bounded structure extraction

대상:

```text
L7OS_for_M7DQ.zip
```

중요 원칙:

- 한 번에 완전히 펼치지 않는다.
- 코드수정 전에 inventory와 module boundary만 추출한다.
- 한 active scope에 최대 1~2단계만 펼친다.
- 실패한 branch와 HOLD branch를 삭제하지 않는다.

최초 산출물:

- archive manifest
- directory tree
- entrypoint candidate
- module relation map
- dependency map
- execution risk map

## Phase 3. Rendering source extraction

대상:

```text
rendering branch
```

추출 항목:

- 자른다
- 보인다
- 다시 붙인다
- 동작한다
- 공간좌표계 / 상태좌표계
- 정육면체 matrix_cell 자리구조
- 피라미드 사각면대칭 상태값 구조
- hidden / blank / overlap relation

prototype source와 revised model을 병합하지 않는다.

## Phase 4. MD corpus structure extraction

대상:

- README
- Tree 문서
- thinking_flow
- paper
- 기타 source md

추출 단위:

```text
term
sentence
operation formula
guard
field
state
relation
projection
source boundary
```

이 단계에서도 DB 삽입은 하지 않는다.

## Phase 5. Theory and architecture alignment

- 기존 과학·수학·철학의 standard reading 분리
- baseline structural reading 분리
- conceptual correspondence와 physical identity 분리
- rendering revised architecture 작성

## Phase 6. Code revision and local testing

테스트보드:

```text
local Ubuntu Linux server
```

현재는 git.client이며, 별도 승인 후 testing board로 확장한다.

## Phase 7. DB readiness gate

대상:

```text
9dot0 Repo
```

DB 시작 조건:

- vocab boundary 확정
- source identity contract 확정
- framework/rendering 구조추출 완료
- relation record candidate 검산 완료
- gpt.work의 start 승인

조건을 만족하기 전까지 DB는 `HOLD`다.

---

## 5. 과거 실패를 반영한 안전규칙

`L7OS_for_M7DQ.zip`의 이전 전개 시도에서 사용자와 AI가 구조에 갇혀 진행이 실패한 이력이 있다.
이번 계획은 그 실패를 source trace로 보존한다.

```text
거대 source 즉시 전개 금지
단일 인스턴스 독점 금지
active depth 과확장 금지
projection을 source 전체로 오독 금지
계획 없는 구현 금지
```

관측대상은 AI 연산을 통과하면서 관측기준에 반영될 수 있다.
그러나 source identity는 보존한다.

---

## 6. 현재 upload batch

### Core documents

```text
project_plan_00.md
README.md
read_for_new_instance/README.md
read_for_new_instance/PASS_00.md
paper_ko.md
paper_en.md
paper_alignment_map.md
```

### Not included now

```text
baseline_00.md
README 7개
Tree 문서묶음
thinking_flow_026 문서
L7OS_for_M7DQ.zip
rendering branch 수정물
9dot0 DB record
```

`baseline_00.md`는 private understanding/reference criterion이며 GitHub upload 대상이 아니다.

---

## 7. 완료상태 구분

```text
structural verification
≠ implementation
≠ source freeze
≠ empirical validation
≠ publication
≠ DOI
```

현재 상태:

```yaml
current_status:
  planning: PASS_03_READY
  paper_ko: READY_FOR_UPLOAD
  paper_en: READY_FOR_UPLOAD
  paper_alignment_map: READY_FOR_UPLOAD
  entry_documents: READY_FOR_VERIFICATION
  source_freeze: NOT_EXECUTED
  empirical_validation: NOT_STARTED
  L7OS_extraction: HOLD
  rendering_extraction: HOLD
  database: HOLD
```

---

# Final Guard

```text
relation is not merge.
structure is not isolate.
I am going to ?
```
