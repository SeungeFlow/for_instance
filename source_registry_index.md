# gpt_direct source_registry_index.md

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

## 1. source registry identity

instance: gpt.direct
branch: gpt_direct
document_role: source_registry_index

---

## 2. source identity 원칙

source identity는 gpt.direct branch의 중심 기준장이다.

어떤 문서가 어디에서 왔는지 모르면 DB에 넣으면 안 된다.

source identity required: YES

---

## 3. source_registry_value_guard

raw_url: ONLY_IF_KNOWN
commit_sha: ONLY_IF_VERIFIED
repo_branch_path: DECLARED_OR_VERIFIED_STATUS_REQUIRED
unknown_value: UNKNOWN
principle: 값은 값이다.

추측값은 source_registry에 넣지 않는다.

모르는 값은 UNKNOWN으로 둔다.

UNKNOWN은 실패가 아니다.

UNKNOWN을 값처럼 꾸미는 것이 실패다.

---

## 4. source registry metadata fields

source_id:
source_type:
source_repo:
source_branch:
source_path:
raw_url:
commit_sha:
source_status:
declared_by:
verified_by:
accepted_by:
implemented_by:
relation_to_primary:
read_status:
notes:
final_guard:

---

## 5. source status vocabulary

DECLARED:
표시되었으나 검증되지 않음

VERIFIED:
검증됨

ACCEPTED:
공동협의체에서 수용됨

IMPLEMENTED:
gpt.gitwork 실행 이후 실제 GitHub에 배치됨

UNKNOWN:
현재 모름

HOLD:
보류

---

## 6. 초기 source 후보

현재는 실제 source registry body를 생성하지 않는다.

초기에는 source registry의 구조만 둔다.

current_status: INDEX_ONLY
source_body_creation: NO
actual_file_creation: NO

향후 gpt.work가 placement packet을 만들고 gpt.gitwork가 source field를 인식한 뒤, source registry body가 생성될 수 있다.

---

## 7. source registry relation guard

source registry는 original source를 대체하지 않는다.

raw_url은 source relation이다.

commit_sha는 source identity 강화를 위한 값이다.

snapshot은 original을 대체하지 않는다.

relation is not merge.

final_guard: relation is not merge
