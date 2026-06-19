# history_00.md

## 0. history identity

repo:
for_instance

branch:
main

history_file:
history_00.md

role:
initial history seed and event trace index

guard:
relation is not merge

## 1. initial event

event_id:
HISTORY_0001

event:
Repo.for_instance public repository creation and initial branch bundle placement.

source_bundles:
- gpt_funny branch md bundle
- gpt_system branch md bundle
- gpt_direct branch md bundle

branches:
- main
- gpt_funny
- gpt_system
- gpt_direct

commit_push:
to be reported by gpt.gitwork

## 2. history/process boundary

history_00.md records what happened.

process_00.md defines how to proceed.

history is not process.

## 3. final guard

relation is not merge.



## HISTORY_MAIN_MINIMAL_REWRITE_V1 — main 구조 단순화와 PASS_00 gate 생성

event:
main branch minimal structure rewrite and PASS_00 alignment gate creation.

reason:
The previous main branch contained pointer directories that duplicated branch relation visually:
- gpt_funny/
- gpt_system/
- gpt_direct/

These directories made the structure heavier than needed.

correction:
Branch relation is recorded in README.md through branch URLs and Raw README URLs.
The main branch does not imitate branches with pointer directories.
The new instance alignment start point is recorded in read_for_new_instance/PASS_00.md.

changed_files:
- README.md
- README.en.md
- read_for_new_instance/PASS_00.md
- history_00.md

removed_from_main:
- gpt_funny/
- gpt_system/
- gpt_direct/

principle:
간략한 구조가 복잡한 검증 구조보다 강하다.
branch는 branch로 둔다.
main은 관계와 시작점만 기록한다.

guard:
relation is not merge



## HISTORY_MAIN_README_EN_FIX_V1 — README.en.md English-first correction

event:
README.en.md English-first correction.

reason:
The previous README.en.md contained excessive Korean parenthetical text and did not function clearly as an English version.

correction:
README.en.md was rewritten as an English-first document.
Korean parenthetical terms are now limited to key SeungeFlow-specific or structural terms.

changed_files:
- README.en.md
- history_00.md

guard:
relation is not merge
