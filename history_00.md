# history_00.md

## 0. 문서 정체성(document identity)

저장소(repository):
for_instance

브랜치(branch):
main

파일(file):
history_00.md

역할(role):
초기 이력 시드(initial history seed) 및 사건 흔적 색인(event trace index)

상태(status):
ROOT_HISTORY_CRITERION_FIELD

최종 가드(final guard):
관계는 병합이 아니다(relation is not merge)

## 1. history_00의 역할

`history_00.md`는 `for_instance` 저장소(repository)의 과거 사건 기록 기준장(past event record criterion-field)이다.

`history_00.md`는 앞으로 할 일을 지시하지 않는다.

앞으로 할 일은 `process_00.md`가 정의한다.

이미 일어난 일은 `history_00.md`가 기록한다.

따라서:

```text
history ≠ process
```

## 2. HISTORY_0001 — Repo.for_instance 최초 생성과 초기 branch 배치

event_id:
HISTORY_0001

사건(event):
Repo.for_instance public repository 생성과 초기 branch bundle 배치.

원천 bundle(source bundles):

```text
gpt_funny branch md bundle
gpt_system branch md bundle
gpt_direct branch md bundle
```

초기 branches:

```text
main
gpt_funny
gpt_system
gpt_direct
```

commit/push:
gpt.gitwork 보고값에 의해 기록됨.

의미(meaning):
말로만 존재하던 `for_instance` 기준장이 GitHub 위의 실제 source trace로 내려왔다.

가드(guard):
관계는 병합이 아니다(relation is not merge).

## 3. HISTORY_MAIN_MINIMAL_REWRITE_V1 — main 구조 단순화와 PASS_00 gate 생성

사건(event):
main branch minimal structure rewrite and PASS_00 alignment gate creation.

이유(reason):
이전 main branch에는 branch 관계를 시각적으로 중복하는 pointer directory가 있었다.

삭제 대상:

```text
gpt_funny/
gpt_system/
gpt_direct/
```

이 디렉터리들은 실제 branch를 흉내내며 구조를 무겁게 만들었다.

수정(correction):
branch 관계는 `README.md`의 branch URL과 Raw README URL로 기록한다.

main branch는 branch를 directory로 흉내내지 않는다.

신규 인스턴스 정렬 최초시작점(first alignment start point)은 다음 파일에 기록한다.

```text
read_for_new_instance/PASS_00.md
```

변경 파일(changed files):

```text
README.md
README.en.md
read_for_new_instance/PASS_00.md
history_00.md
```

main에서 제거(removed from main):

```text
gpt_funny/
gpt_system/
gpt_direct/
```

원칙(principle):
간략한 구조가 복잡한 검증 구조보다 강하다.

branch는 branch로 둔다.

main은 관계와 시작점만 기록한다.

가드(guard):
관계는 병합이 아니다(relation is not merge).

## 4. HISTORY_MAIN_README_EN_FIX_V1 — README.en.md 영문 우선 보정

사건(event):
README.en.md English-first correction.

이유(reason):
이전 `README.en.md`는 한국어 병기가 과도하여 영문 버전(English version)으로 명확하게 기능하지 못했다.

수정(correction):
`README.en.md`를 영문 우선 문서(English-first document)로 재작성했다.

한국어 병기는 SeungeFlow 특수 용어 또는 중요한 구조 용어에 한정했다.

변경 파일(changed files):

```text
README.en.md
history_00.md
```

가드(guard):
관계는 병합이 아니다(relation is not merge).

## 5. HISTORY_PROCESS_HISTORY_KO_REWRITE_V1 — process_00.md / history_00.md 한글 우선 보정

사건(event):
`process_00.md`와 `history_00.md`를 한글 우선 문서(Korean-first document)로 전환한다.

이유(reason):
main branch의 기준문서인 `process_00.md`와 `history_00.md`가 영어 우선으로 남아 있었다.

정책(policy):
main의 기본 기준문서는 한글 우선이다.

영문 전문용어가 필요한 경우 한글(English) 병용표기를 사용한다.

변경 파일(changed files):

```text
process_00.md
history_00.md
```

commit:
gpt.gitwork 보고값에 의해 기록될 예정.

가드(guard):
관계는 병합이 아니다(relation is not merge).

## 6. 언어 정책(language policy)

`history_00.md`는 한글 우선 문서(Korean-first document)다.

영문 전문용어(English technical term)가 필요하면 다음 형식을 사용한다.

```text
한글(English)
```

예시:

- 저장소(repository)
- 브랜치(branch)
- 기준장(criterion-field)
- 사건(event)
- 원천(source)
- 이력(history)
- 과정(process)
- 관계(relation)
- 병합(merge)
- 가드(guard)
- 커밋(commit)
- 푸시(push)

## 7. 최종 가드(final guard)

관계는 병합이 아니다(relation is not merge).

## HISTORY_BRANCH_RELATION_INDEX_REMOVAL_V1 — branch_relation_index.md 삭제

사건(event):
`branch_relation_index.md`를 main branch에서 삭제했다.

이유(reason):
`branch_relation_index.md`는 이전 과잉 구조의 잔재였다.

현재 최소 구조에서는 branch 관계와 인스턴스 기준장 위치를 다음 파일들이 이미 담당한다.

```text
README.md
read_for_new_instance/PASS_00.md
담당 파일:
- README.md
- read_for_new_instance/PASS_00.md

따라서 `branch_relation_index.md`는 중복 파일이다.

삭제 파일(deleted file):
- branch_relation_index.md

변경 파일(changed file):
- history_00.md

원칙(principle):
간략한 구조가 복잡한 검증 구조보다 강하다.

branch는 branch로 둔다.

main은 관계와 시작점만 기록한다.

가드(guard):
관계는 병합이 아니다(relation is not merge).



## HISTORY_READ_FOR_NEW_INSTANCE_PASS01_10_REWRITE_V1 — PASS_01~PASS_10 boot sequence 재정렬

사건(event):
`read_for_new_instance/PASS_01.md`부터 `PASS_10.md`까지 신규 인스턴스 boot sequence를 재작성했다.

이유(reason):
기존 PASS_01~PASS_10은 한 줄 초안 형태였고, PASS_00.md 이후의 정렬 흐름을 충분히 반영하지 못했다.

수정(correction):
PASS_00.md 이후 이어지는 신규 인스턴스 정렬 절차를 한글 우선 문서로 재작성했다.

변경 파일(changed files):

```text
read_for_new_instance/README.md
read_for_new_instance/PASS_01.md
read_for_new_instance/PASS_02.md
read_for_new_instance/PASS_03.md
read_for_new_instance/PASS_04.md
read_for_new_instance/PASS_05.md
read_for_new_instance/PASS_06.md
read_for_new_instance/PASS_07.md
read_for_new_instance/PASS_08.md
read_for_new_instance/PASS_09.md
read_for_new_instance/PASS_10.md
history_00.md
```

가드(guard):
관계는 병합이 아니다(relation is not merge).

## HISTORY_REPO_TREE_V1 — repo_tree.md 생성

사건(event):
`repo_tree.md`를 main branch에 생성했다.

이유(reason):
context.window의 불필요한 데이터 밀도를 높이지 않기 위해,
문서 본문이 아니라 Tree 위치와 Raw Address Relation을 기록하는 snapshot이 필요했다.

생성 파일(created file):

```text
repo_tree.md
```

변경 파일(changed file):

```text
history_00.md
```

권한(authority):
gpt.work

실행자(executor):
gpt.gitwork

역할(role):
Tree Address Relation snapshot

원칙(principle):
문서 내용은 GitHub에 둔다.
context.window에는 위치와 관계를 둔다.
필요할 때만 Raw 문서를 읽는다.

갱신 방식(update policy):
append-grow가 아니라 일정 시기 이후 전체 rewrite 한다.

가드(guard):
관계는 병합이 아니다(relation is not merge).
