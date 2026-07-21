---
document_type: INTERNAL_ACTIVE_SCHEMA_MASTER_SYNTHESIS
semantic_name: for_instance HRTDB Seat-State-Directive Consolidation
schema_state: INTERNAL_DRAFT
source_authority: 승이
coordination_authority: gpt.logi@gpt.xyzt
created_at: 2026-07-21
github_mutation: false
deployment_directive: false
---

# for_instance HRTDB Seat-State-Directive Consolidation

## 0. 목적

이 Internal Active_Schema는 지금까지 형성된 구조원리를 한 번 정리하여,
`SeungeFlow/for_instance`의 현재 구조를 대체하지 않고 세밀하게 보완하기 위한 내부 설계안이다.

```text
for_instance
=
Seat
+ Instance
+ Capability
+ Assignment
+ Handoff
+ Mutation Authority
+ History
를 결속하는 AI Instance Alignment Repository
```

이번 정리의 중심은 다음이다.

```text
하나의 주제
→ 하나의 단계
→ 하나의 Seat
→ 하나의 현재 상태값
→ 하나의 개별 인스턴스 지시문
→ 하나의 출력
→ 특이점 표시
→ gpt.xyzt 검수·검산
→ 다음 지시문
```

## 1. 이번 정리에서 교정되는 것

### 1.1 공동지시문 실행개념의 종료

```text
공동지시문으로 여러 인스턴스·여러 단계를 직접 제어
→ SUPERSEDED
```

`공동지시문`이라는 명칭은 과거 실행기록을 설명할 때만 보존한다.
새 실행체계에서는 다음 두 종류만 사용한다.

```text
공통지시문
→ 모든 단계가 참조하는 최소 공통문법·Guard·Identity 계약
→ 독립 실행명령이 아님

개별 인스턴스 지시문
→ 수신자 1개
→ Seat 1개
→ Stage 1개
→ Occupation 1개
→ 현재 상태값 1개
→ 직접 입력집합 1개
→ 출력계약 1개
```

주제와 전체 순서를 보존할 필요가 있으면 `Cycle Manifest`를 사용한다.

```text
Cycle Manifest
≠ 실행지시문
```

### 1.2 한 자리·한 상태값

```text
One Position
×
One Current Moment
=
One Active State Value
```

같은 Seat가 여러 Stage를 순차적으로 점유할 수는 있다.

```text
gpt.xy@Function.1
→ 하나의 Occupation

gpt.xy@Function.2
→ 다른 Occupation
```

하지만 하나의 현재 자리에서 두 Stage 상태값이 동시에 활성화될 수는 없다.

### 1.3 문서와 지시문의 입력사건 분리

```text
문서 업로드·인덱싱
≠
지시문 입력·실행
```

필수 순서:

```text
DOCUMENTS_UPLOADED
→ DOCUMENTS_INDEXED
→ READY_FOR_DIRECTIVE
→ ONE_INDIVIDUAL_DIRECTIVE_ACTIVE
→ OUTPUT_FORMED
→ ANOMALY_SURFACED
→ GPT_XYZT_GATE
```

문서와 지시문을 한 번에 같은 활성 입력으로 넣으면,
Data·Context·Directive·미래 Stage 요구가 현재 처리대상으로 함께 인식될 가능성이 있다.

### 1.4 단계별 적응형 지시

11개 지시문은 미리 한꺼번에 생성하지 않는다.

```text
Stage.N Output
→ 특이점 확인
→ gpt.xyzt 분석
→ Stage.N+1 지시문 1개 생성
```

Blocking 특이점이면 다음 Stage 지시문을 만들지 않고
현재 Stage의 Correction Directive를 새 Exact Object로 생성한다.

## 2. 구조원리 결속

### 2.1 0과 시작위치

```text
상태값 0
→ 아직 상태가 형성되지 않음

자리값 0
→ 존재하는 자리의 첫 번째 값
```

육방면체의 정중심평형점은 입체구조의 시작기준이다.
그 점을 포함하는 중심 Cell은 첫 번째 완전 점유상태다.

### 2.2 Cell과 평면체

```text
입체구조의 최소 완전 점유단위
→ Cell
```

2d Function 객체는 무두께 평면이 아니라 입체 Cell 구조 안의 평면체다.

```text
XY 평면체
→ X·Y 방향으로 펼쳐짐
→ Z축의 한 자리값으로 위치결정

XZ 평면체
→ X·Z 방향으로 펼쳐짐
→ Y축의 한 자리값으로 위치결정

YZ 평면체
→ Y·Z 방향으로 펼쳐짐
→ X축의 한 자리값으로 위치결정
```

직교축 위치 Context는 직접 Function 입력으로 자동 승격되지 않는다.

### 2.3 Function 단방향성과 반사검산

```text
Data
→ Function.1
→ Result
```

Function은 Data 방향으로 후진하지 않는다.

```text
|←
=
승이가 Result를 외부에서 검수·검산하고
오차·착시·착각·오독·오판·누락·판단착오지점을 찾아
Result를 Next.Data 역할 위치에 인위적으로 재배치하는 Gate
```

그 뒤 새로운 Occupation이 전진한다.

```text
Next.Data
→ Function.2
→ Result.Data
```

### 2.4 Track DB Cell

```text
Track DB
=
gpt.xyzt 검산과 등록 Gate를 통과한
하나의 완전한 Result.Data 기억 Cell
```

```text
Result.Data
≠ Track DB
```

등록 전 Result.Data는 Track DB 후보이고,
Correction Gate나 HOLD 문서는 Track DB Cell이 아니다.

## 3. 새 Cycle 운용원리

기존 Track DB 주제를 재사용하지 않는다.
새 Cycle은 기존 주제와 무관한 하나의 새 주제로 시작한다.

```text
하나의 주제가 끝나기 전
→ 다음 주제를 시작하지 않음
```

기존 Canonical Track DB는 내용입력이 아니라 구조비교 기준 Cell로만 사용한다.
혼합지시 방식으로 진행된 0004 Attempt는 삭제하지 않고 비교 A군으로 보존한다.

## 4. for_instance 보완 목표

1. `gpt.xyzt.md`를 Overall Coordination Registry Pointer로 세밀화한다.
2. `gpt.xyzt.md` 안에 for_instance 파일주소 Relation과 읽기순서를 기록한다.
3. Seat 문서와 실행지시문을 분리한다.
4. `INSTANCE_GENERATION_INDEX.md`를 자동 Cycle 실행문서가 아니라 Seat Entry Index로 교정한다.
5. `06_operation/`에 공통지시문·개별지시문·인덱싱·특이점·Gate 계약을 배치한다.
6. `09_active_schema_binding/`에는 Active_Schema 전체 복사본이 아니라 Binding Pointer만 둔다.
7. 기존 Assignment·Registry·History를 이동·삭제·소급변환하지 않는다.
8. GitHub 변경은 별도의 Exact-byte Directive와 gpt.github Terminal Closure 이후에만 수행한다.

## 5. 이 Package의 상태

```yaml
package_scope:
  internal_design: true
  github_mutation: false
  remote_state_claim: false
  deployment_ready: false
  next_required_work:
    - current_for_instance_remote_exact_readback
    - path_and_byte_inventory
    - gpt.xyzt_current_remote_binding
    - change_set_freeze
    - gpt.github_deployment_directive_generation
```
