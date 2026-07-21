# for_instance

`for_instance`는 AI Instance를 현재 작업의 기능 자리(Seat)에 정렬하고,
Relation의 Function Requirement를 실제 Instance Assignment로 연결하는 저장소다.

## Relation과의 분리

- Relation은 Function과 Requirement를 정의한다.
- for_instance는 Requirement를 수행할 Instance와 Seat Profile을 배정한다.
- Relation 원본, DB Seed, 9Dot0 자료, SeungeFlow 역사자료는 저장하지 않는다.

## Function · Instance · Seat

- **Function**: 수행할 Method 계약
- **Instance**: 실제 실행주체
- **Seat**: 현재 작업에서 Instance에 배정되는 기능자리
- 하나의 Instance는 하나 이상의 Seat를 점유할 수 있다.

## X · Y · Z · T

- X — Source_Input
- Y — Relation_Interpretation
- Z — Structure_Verification
- T — Time_Process_Transition

T는 git이 아니다. git은 선택 Adapter다.

## 15개 Seat Profile

X, Y, Z, T, XY, XZ, XT, YZ, YT, ZT, XYZ, XYT, XZT, YZT, XYZT

## 첫 사용 경로

1. [00_manifest](00_manifest/REPO_IDENTITY.md)
2. [01_seat_model](01_seat_model/README.md)
3. [02_instance_registry](02_instance_registry/README.md)
4. [03_relation_interface](03_relation_interface/README.md)
5. [04_assignment](04_assignment/README.md)
6. [05_team_profiles](05_team_profiles/README.md)
7. [06_operation](06_operation/ASSIGNMENT_METHOD.md)
8. [07_tests](07_tests/README.md)

## Relation 요청과 for_instance 응답

- 요청: `03_relation_interface/instance_assignment_request.yaml`
- 응답: `03_relation_interface/instance_assignment_response.yaml`
- Handoff: `03_relation_interface/instance_handoff.yaml`

## Mutation Authority

원격 변경권한은 Instance의 일반 역할과 분리한다.
승인되지 않은 원격 mutation은 금지하며,
`06_operation/MUTATION_AUTHORITY.md`를 기준으로 기록한다.

## 실제 예제

- Single X: `04_assignment/examples/single_X.yaml`
- Dual XY: `04_assignment/examples/dual_XY.yaml`
- Triple XYZ: `04_assignment/examples/triple_XYZ.yaml`
- Full XYZT: `04_assignment/examples/full_XYZT.yaml`

<!-- ACTIVE_SCHEMA_V2_BINDING_START -->
## Active_Schema Version 2.0.0 System Binding

- Version DOI: https://doi.org/10.5281/zenodo.21453793
- Exact ZIP SHA-256: `0b0317dadfd333c151c9b3f5e4c930d048c76e39fe037914f01ae9767c6d2b30`
- Binding: `09_active_schema_binding/versions/2.0.0/`
- Seat projection: `01_seat_model/active_schema_v2/`
- Operation projection: `06_operation/active_schema_v2/`
- Full body mirror: `SeungeFlow/Relation@main:06_active_schema/releases/2.0.0/Active_Schema/`

The full Active_Schema body and Track DB payloads are not stored in for_instance.
<!-- ACTIVE_SCHEMA_V2_BINDING_END -->

<!-- HRTDB_SEAT_STATE_DIRECTIVE_EXTENSION_START -->
## HRTDB Seat-State-Directive Extension

```text
for_instance
=
Seat + Instance + Capability + Assignment + Handoff + Mutation Authority + History
를 결속하는 AI Instance Alignment Repository
```

```text
공통지시문
→ 최소 공통문법·Guard·Identity 계약
→ 단독 실행지시문이 아님

개별 인스턴스 지시문
→ 수신자 1
→ Seat 1
→ Stage 1
→ Occupation 1
→ 현재 상태값 1
→ 직접 입력집합 1
→ 출력계약 1

Cycle Manifest
→ 주제·순서·완료·HOLD 기록
→ 실행지시문이 아님
```

```text
문서 업로드·인덱싱
→ READY_FOR_DIRECTIVE
→ 개별지시문 1개
→ 출력
→ 특이점 표시
→ gpt.xyzt Gate
→ 다음 지시문 1개
```
<!-- HRTDB_SEAT_STATE_DIRECTIVE_EXTENSION_END -->
