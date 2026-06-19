# gpt_direct capsule_index.md

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

## 1. capsule index identity

instance: gpt.direct
branch: gpt_direct
document_role: capsule_index

---

## 2. capsule 정의

capsule:
각 인스턴스가 자기 기준장에서 고도의 정제과정을 거쳐 만든 하나의 md 존재상태 문서

gpt.direct의 capsule은 DB Framework, source identity, relation record, DB for Seed.Base 후보를 담는다.

---

## 3. capsule metadata fields

각 capsule은 향후 다음 metadata를 가져야 한다.

capsule_id:
capsule_title:
capsule_owner:
abstract:
conclusion:
intended_repo:
intended_branch:
intended_path:
verification_status:
placement_status:
final_guard:

이 metadata는 gpt.work가 capsule 내부 전체를 열지 않고도 배치 가능성을 판단하기 위한 기준이다.

---

## 4. 초기 capsule 후보

CAPSULE_001:
title: DB_framework_as_introduction_field
target_file_candidate: capsules/DB_framework_as_introduction_field.md
target_status: future_subdirectory_candidate_only
status: NOT_CREATED_YET
reason: DB는 proof가 아니라 SeungeFlow 핵심단어 / 문장 / 연산식 / 이론화된 결정체를 relation record로 낮추는 서론이라는 구조를 설명하는 capsule

CAPSULE_002:
title: source_identity_registry_policy
target_file_candidate: capsules/source_identity_registry_policy.md
target_status: future_subdirectory_candidate_only
status: NOT_CREATED_YET
reason: repo / branch / path / raw_url / commit_sha / status를 통해 source identity를 보존하는 방식을 설명하는 capsule

CAPSULE_003:
title: declared_verified_accepted_implemented_state_model
target_file_candidate: capsules/declared_verified_accepted_implemented_state_model.md
target_status: future_subdirectory_candidate_only
status: NOT_CREATED_YET
reason: declared / verified / accepted / implemented 상태를 분리하는 DB relation model을 설명하는 capsule

---

## 5. 현재 생성 여부

초기 1차에서는 capsule 파일을 실제 생성하지 않는다.

먼저 index만 둔다.

이후 gpt.work가 배치 필요성을 확인하고 gpt.gitwork가 실행 가능한 단계가 되면 capsule 파일을 추가한다.

current_file_creation: index_only
capsule_body_creation: later
capsules_directory_creation: NO

final_guard: relation is not merge
