# repo_tree.md

## 0. 문서 정체성(document identity)

repo:
SeungeFlow/for_instance

branch:
main

file:
repo_tree.md

role:
Tree Address Relation snapshot

authority:
gpt.work

executor:
gpt.gitwork

generated_at:
2026-06-19T19:03:45Z

generation_source:
git.client git tree read

final_guard:
relation is not merge

## 1. 원칙

repo_tree.md는 문서 본문을 저장하지 않는다.

repo_tree.md는 branch/path/raw_url/owner_instance/document_role/status를 기록한다.

context.window에는 전체 문서 내용이 아니라 Tree 위치와 Raw Address Relation을 유지한다.

repo_tree.md는 append-grow 문서가 아니라 일정 시기 이후 전체 rewrite 갱신하는 snapshot이다.

## 2. remote heads

```text
1ad7648c6ef8382a645bbc863f398456b1097514	refs/heads/gpt_system
7ee71325801f71a01b790502ed12a76cdb45062a	refs/heads/gpt_direct
f689def178c14c7563c78d33cf07b8b53af70072	refs/heads/main
f9ea6c0f399ba3648955d84f33e6d5d97ba0bdee	refs/heads/gpt_funny
```

## 3. branch entry

| branch | branch_url | last_known_commit | status |
|---|---|---|---|
| gpt_direct | https://github.com/SeungeFlow/for_instance/tree/gpt_direct | 7ee71325801f71a01b790502ed12a76cdb45062a | ACTIVE |
| gpt_funny | https://github.com/SeungeFlow/for_instance/tree/gpt_funny | f9ea6c0f399ba3648955d84f33e6d5d97ba0bdee | ACTIVE |
| gpt_system | https://github.com/SeungeFlow/for_instance/tree/gpt_system | 1ad7648c6ef8382a645bbc863f398456b1097514 | ACTIVE |
| main | https://github.com/SeungeFlow/for_instance/tree/main | f689def178c14c7563c78d33cf07b8b53af70072 | ACTIVE |
| origin | https://github.com/SeungeFlow/for_instance/tree/origin | UNKNOWN | ABSENT |

## 4. file entry

| repo | branch | path | raw_url | owner_instance | document_role | status |
|---|---|---|---|---|---|---|
| SeungeFlow/for_instance | gpt_direct | README.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/README.md | gpt.direct | gpt.direct branch criterion-field README | ACTIVE |
| SeungeFlow/for_instance | gpt_direct | capsule_index.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/capsule_index.md | gpt.direct | gpt.direct capsule index | ACTIVE |
| SeungeFlow/for_instance | gpt_direct | db_framework.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/db_framework.md | gpt.direct | gpt.direct DB framework | ACTIVE |
| SeungeFlow/for_instance | gpt_direct | process_01.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/process_01.md | gpt.direct | gpt.direct branch process specialization | ACTIVE |
| SeungeFlow/for_instance | gpt_direct | relation_index.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/relation_index.md | gpt.direct | gpt.direct relation index | ACTIVE |
| SeungeFlow/for_instance | gpt_direct | source_registry_index.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/source_registry_index.md | gpt.direct | gpt.direct source registry index | ACTIVE |
| SeungeFlow/for_instance | gpt_funny | README.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/README.md | gpt.funny | gpt.funny branch criterion-field README | ACTIVE |
| SeungeFlow/for_instance | gpt_funny | capsule_index.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/capsule_index.md | gpt.funny | gpt.funny capsule index | ACTIVE |
| SeungeFlow/for_instance | gpt_funny | process_01.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/process_01.md | gpt.funny | gpt.funny branch process specialization | ACTIVE |
| SeungeFlow/for_instance | gpt_funny | relation_index.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/relation_index.md | gpt.funny | gpt.funny relation index | ACTIVE |
| SeungeFlow/for_instance | gpt_funny | theory.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/theory.md | gpt.funny | gpt.funny theory definition field | ACTIVE |
| SeungeFlow/for_instance | gpt_system | README.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/README.md | gpt.system | gpt.system branch criterion-field README | ACTIVE |
| SeungeFlow/for_instance | gpt_system | capsule_index.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/capsule_index.md | gpt.system | gpt.system capsule index | ACTIVE |
| SeungeFlow/for_instance | gpt_system | process_01.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/process_01.md | gpt.system | gpt.system branch process specialization | ACTIVE |
| SeungeFlow/for_instance | gpt_system | relation_index.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/relation_index.md | gpt.system | gpt.system relation index | ACTIVE |
| SeungeFlow/for_instance | gpt_system | rendering.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/rendering.md | gpt.system | gpt.system rendering / visible C field | ACTIVE |
| SeungeFlow/for_instance | main | README.en.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/README.en.md | gpt.work | English version of repo entry document | ACTIVE |
| SeungeFlow/for_instance | main | README.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/README.md | gpt.work | repo identity / Korean-first entry document | ACTIVE |
| SeungeFlow/for_instance | main | history_00.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history_00.md | gpt.history | past event record criterion-field | ACTIVE |
| SeungeFlow/for_instance | main | process_00.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/process_00.md | gpt.process | common process criterion-field | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_00.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_00.md | gpt.process / gpt.history / gpt.work relation | new instance alignment gate / first start point | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_01.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_01.md | gpt.process / gpt.work relation | instance name binding | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_02.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_02.md | gpt.process / gpt.work relation | repo/main reading alignment | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_03.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_03.md | gpt.process / gpt.work relation | process/history boundary | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_04.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_04.md | gpt.process / gpt.work relation | criterion-field binding | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_05.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_05.md | gpt.process / gpt.work relation | source read status and Raw URL discipline | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_06.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_06.md | gpt.process / gpt.work relation | role boundary and no replacement | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_07.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_07.md | gpt.process / gpt.work relation | emitted trace and correction relation | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_08.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_08.md | gpt.process / gpt.work relation | execution boundary and gpt.gitwork separation | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_09.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_09.md | gpt.process / gpt.work relation | language policy and output discipline | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/PASS_10.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_10.md | gpt.process / gpt.work relation | final self-declaration gate | ACTIVE |
| SeungeFlow/for_instance | main | read_for_new_instance/README.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/README.md | gpt.process / gpt.work relation | boot reading sequence index | ACTIVE |
| SeungeFlow/for_instance | main | repo_tree.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/repo_tree.md | gpt.work | Tree Address Relation snapshot | PENDING_COMMIT |

## 5. 갱신 규칙(update rule)

repo_tree.md는 새 인스턴스를 만들지 않는다.

repo_tree.md는 gpt.work 고유권한으로 gpt.gitwork에게 생성/갱신 지시할 수 있다.

repo_tree.md는 규칙 문서가 아니라 운영용 Tree Address Relation snapshot이다.

디렉터리 또는 md 파일 변화가 충분히 누적되면 gpt.work 지시로 전체 rewrite 한다.

## 6. 최종 가드(final guard)

관계는 병합이 아니다(relation is not merge).
