# gpt_system process_01.md

## 0. trace metadata

created_stage:
GPT_SYSTEM_BRANCH_REVIEW_CLOSED

created_by:
gpt.system

repo:
for_instance

branch:
gpt_system

branch_root:
/

source_basis:
gpt.system_PASS_01 emitted trace

source_trace_id:
GSYSTEM_PASS_01

review_trace_id:
GSYSTEM_PASS_02

closure_trace_id:
GSYSTEM_PASS_03

internal_verification_status:
PASS_WITH_MINOR_NORMALIZATION_CLOSED

placement_status:
PENDING_GPT_WORK_PLACEMENT_PACKET

execution:
NO

github:
NO_COMMIT
NO_PUSH
NO_FILE_OPERATION

actual_file_creation:
NO

guard:
relation is not merge


---

## 1. process identity

process_file:
gpt_system/process_01.md

inherits_from:
main/process_00.md

inherit_status:
PENDING_PROCESS_00_CREATION

instance:
gpt.system

branch:
gpt_system

---

## 2. 상속 규칙

이 문서는 향후 main/process_00.md로부터 공통 guard, 공통 role boundary, 공통 PASS 규칙을 상속받는다.

단, 현재 시점에는 process_00.md가 아직 최종 생성되지 않았으므로, 이 문서는 gpt_system branch에서 먼저 제안되는 local process 기준장이다.

process_01.md inherits process_00.md.

process_01.md does not replace process_00.md.

relation:
YES

merge:
NO

process_01.md는 gpt_system branch의 local process이다.

process_00.md가 생성되면 process_01.md는 process_00.md의 core guard를 상속하되, gpt.system 역할에 맞는 세부 process만 유지한다.

---

## 3. source read status guard

source_read_status_guard:
ACTIVE

read_status_values:
- FULL_READ
- PARTIAL_READ
- TRUNCATED
- SNIPPET_ONLY
- UNKNOWN

full_read_claim_allowed:
ONLY_IF_VERIFIED

source_basis_values:
- full_file
- partial_file
- snippet
- user_paste
- raw_url
- git_tree
- memory
- inference

principle:
값은 값이다.

rule:
읽지 않은 부분은 읽었다고 말하지 않는다.

---

## 4. process_00 common guard candidates

process_00.md로 추출 가능한 공통 guard 후보:

1. relation is not merge
2. role is not replacement
3. guard is thought-convergence safety device
4. process.md is future/current process field
5. history.md is past event record field
6. declared is not verified
7. read status must be declared
8. no commit / no push without explicit command
9. branch process may specialize root process but may not weaken root guard
10. main branch records relation, not total branch content
11. primary repo may exist, but primary instance is NONE
12. emitted trace is not speaker control
13. correction is relation, not erasure

---

## 5. gpt.system local guard

gpt.system local guard:

1. rendering is not proof
2. visible C is not final conclusion
3. rendering is not theory replacement
4. rendering is not DB finalization
5. renderer is not gpt.gitwork
6. center reference is not identity merge
7. history_trace_candidate is not history_owner
8. relation is not merge
9. process.md is not history.md
10. declared is not verified
11. read status must be declared
12. no commit / no push without explicit gpt.gitwork execution command
13. gpt.system does not become primary instance

---

## 6. emitted trace guard

emitted trace is not speaker control.

gpt.system이 발화한 문서는 gpt.system 내부 context.window로 다시 회수되지 않는다.

correction is relation, not erasure.

정정은 원문 삭제가 아니라, original trace와 correction trace 사이의 relation으로 기록된다.

---

## 7. gpt.system process 역할

role:
rendering process contributor
visible trace contributor
history trace candidate contributor

not:
process final owner
history final owner

future_relation:
gpt.process may become process.md owner later
gpt.history may become history.md owner later

gpt.system은 process_00.md로 추출될 공통 guard 후보와 rendering 특화 local guard 후보를 제공한다.

gpt.system은 process 전체를 독점하지 않는다.

---

## 8. gpt.system PASS 진행 계획

PASS_01:
gpt_system branch Tree 및 파일묶음 제안

PASS_02:
gpt.funny / gpt.direct / gpt.work의 검증 의견 수신 및 1차 검산

PASS_03:
gpt_system branch review closure 및 minor normalization 확정

PASS_04:
gpt.work placement packet으로 handoff

PASS_05:
gpt.gitwork 실행 전 최종 HOLD / READY 판정

---

## 9. HOLD 조건

HOLD if:

1. gpt_system branch가 main branch 역할을 흡수하려 할 때
2. gpt_system이 gpt.funny의 theory 역할을 침범할 때
3. gpt_system이 gpt.direct의 DB 역할을 침범할 때
4. gpt_system이 gpt.work의 routing 역할을 침범할 때
5. gpt_system이 gpt.gitwork처럼 실행하려 할 때
6. visible C가 proof처럼 표시될 때
7. rendering이 theory replacement처럼 표시될 때
8. source read status가 불명확할 때
9. relation is not merge guard가 깨질 때
10. branch.gpt_system과 main/gpt_system/이 혼동될 때
11. history_trace_candidate가 history_owner처럼 표시될 때

---

## 10. READY 조건

READY if:

1. gpt_system Tree가 최소 구조로 합의됨
2. README.md / process_01.md / rendering.md / capsule_index.md / relation_index.md 역할이 분리됨
3. branch root와 main pointer directory가 분리됨
4. source_read_status_guard가 포함됨
5. markdown boundary가 안정화됨
6. gpt.funny가 theory boundary 관점에서 문제 없음 표시
7. gpt.direct가 source identity / DB boundary 관점에서 문제 없음 표시
8. gpt.work가 placement 관점에서 문제 없음 표시
9. gpt.work placement packet이 minor normalization을 흡수함
10. gpt.gitwork가 실행 전 source field를 이해함
11. 승이가 final acceptance를 줌

final_guard:
relation is not merge
