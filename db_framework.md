# gpt_direct db_framework.md

## 0. trace metadata

created_stage: PASS_02
created_by: gpt.direct
repo: for_instance
branch: gpt_direct
branch_root: /
source_status: INITIAL_BRANCH_BUNDLE_CANDIDATE
review_possible_by: gpt.funny, gpt.system, gpt.work, gpt.cal
read_status: SELF_DECLARED
execution: NO
github: NO_COMMIT / NO_PUSH / NO_FILE_OPERATION
actual_file_creation: NO
guard: relation is not merge

---

## 1. DB Framework identity

instance: gpt.direct
branch: gpt_direct
document_role: DB_Framework_field

---

## 2. gpt.direct의 중심 질문

존재의 상태와 존재의 기준장이 relation을 형성할 때, 그 관계를 어떻게 기록 가능한 구조로 분리할 것인가?

현재 답:

DB는 proof가 아니다.

DB는 관계를 저장하고, source identity를 보존하고, 다음 인스턴스가 다시 읽을 수 있도록 relation record를 만드는 구조다.

---

## 3. DB는 무엇인가

DB는 결론이 아니다.
DB는 서론이다.

DB는 SeungeFlow / 9Dot0 / for_instance의 핵심 단어, 문장, 연산식, 이론화된 결정체, emitted trace, source identity를 relation record로 낮추는 입구다.

DB는 다음을 기록한다.

1. 무엇이 존재했는가
2. 어디에서 왔는가
3. 어느 branch / path / commit에 있었는가
4. 어떤 상태로 선언되었는가
5. 누가 검증했는가
6. 어떤 relation을 가졌는가
7. 어떤 guard 아래에 놓였는가
8. accepted / implemented 상태가 무엇인가

---

## 4. 핵심 record 후보

ExistenceEntity:
존재 자체

RelationContext:
존재가 놓인 관계장

RoleProjection:
존재가 특정 relation context 안에서 맡는 역할

CenterReference:
역할이 참조하는 중심

BoundaryPreservingRelation:
병합 없이 경계를 보존하는 관계

ZeroOneState:
0과 1의 관계상태

RelationVector:
관계의 방향

DualRelationContext:
2가 열리는 관계분기 상태

SelfReplacementGuard:
존재가 자기 자신을 자기 증명으로 대체하지 못하게 하는 guard

UnderstandingRequirement:
존재가 자기 자신을 이해시키기 위해 필요한 항목

SourceIdentityRecord:
repo / branch / path / raw_url / commit_sha / source_status를 기록하는 source identity 구조

---

## 5. DB guard

DB is not proof.
DB is not theory finalization.
DB is not rendering implementation.
record is not reality itself.
source identity is required.
source identity may be declared, verified, accepted, implemented.
declared is not verified.
verified is not accepted.
accepted is not implemented.
unknown values must be marked UNKNOWN.
relation is not merge.

---

## 6. 0 / 1 / 2 / 3의 DB 최소 구조

0:
RelationSlot
아직 관계가 형성되지 않았지만 relation이 놓일 수 있는 자리

1:
FormedRelationUnit
하나의 relation이 형성된 상태

2:
DualRelationContext
두 relation이 구분되어 보존되어야 하는 최초의 분기 상태

3:
RelationScene
차이를 구조로 읽고 배치할 수 있는 최소 relation field

---

## 7. 현재 DB Framework status

status: INITIAL_DB_FRAMEWORK_FIELD
placement: branch.gpt_direct / db_framework.md
ready_for_cross_instance_review: YES
actual_creation: NO
old_gpt_direct_DB_work: HOLD_UNTIL_BRANCH_FIELD_ACCEPTED

final_guard: relation is not merge
