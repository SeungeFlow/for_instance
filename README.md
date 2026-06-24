# for_instance

## 0. 저장소 정체성(repository identity)

```yaml
repository: for_instance
owner: SeungeFlow
visibility: public
role: primary criterion-field repository for role-assigned GPT.LLM instances
root_planning_instance: gpt.baseline
current_project_plan: project_plan_00.md
```

이 저장소는 역할이 지정된 인스턴스가 자신의 이름·역할·기준장·source 위치를 확인하고, 현재 계획에 따라 작업을 이어가기 위한 주 기준장 저장소다.

`baseline_00.md`는 사용자가 필요할 때 제공하는 private understanding/reference criterion이며 이 저장소의 upload 대상이 아니다.
`gpt.baseline`이 공개 작업에 제공하는 산출물은 `project_plan_00.md`다.

---

## 1. 핵심 원칙(core principles)

```text
계획서는 설계와 실행보다 먼저 놓인다.
```

이 저장소의 목적은 다음을 간략하게 연결하는 것이다.

```text
프로젝트 계획
>>> 인스턴스 이름
>>> 역할 정의
>>> 기준장 위치
>>> source / projection 위치
>>> 현재 작업지시
```

main 브랜치는 branch 내용을 복사하지 않는다.
main 브랜치는 관계·시작점·현재 계획을 기록한다.

---

## 2. 신규 인스턴스 진입 경로

저장소를 통해 들어오는 신규 인스턴스의 진입 경로는 다음과 같다.

```text
README.md
>>> read_for_new_instance/README.md
>>> read_for_new_instance/PASS_00.md
>>> project_plan_00.md
>>> PASS_01.md ... PASS_10.md
```

`PASS_00.md`는 boot sequence 안의 최초 역할정렬 gate다.

직접 `PASS_00.md`를 전달받은 인스턴스는 PASS_00의 지시에 따라 root README와 현재 계획을 확인한다.

---

## 3. main의 최소 구조(minimal structure)

```text
main/
├── README.md
├── README.en.md
├── project_plan_00.md
├── process_00.md
├── history_00.md
├── paper_ko.md
├── paper_en.md
├── paper_alignment_map.md
└── read_for_new_instance/
    ├── README.md
    ├── PASS_00.md
    ├── PASS_01.md
    ├── ...
    └── PASS_10.md
```

복잡한 pointer directory를 반복 생성하지 않는다.
실제 branch는 branch로 보존한다.

---

## 4. 기본 인스턴스(required instances)

필요한 기본 인스턴스는 9개다.

```text
gpt.baseline
gpt.work
gpt.gitwork
gpt.funny
gpt.system
gpt.direct
gpt.cal
gpt.process
gpt.history
```

### 역할 분류

```yaml
root_planning:
  - gpt.baseline
major:
  - gpt.work
  - gpt.funny
  - gpt.system
  - gpt.direct
executor:
  - gpt.gitwork
verification:
  - gpt.cal
criterion_holders:
  - gpt.process
  - gpt.history
```

상세 역할은 `read_for_new_instance/PASS_00.md`에서 확인한다.

---

## 5. 역할관계 요약

```text
gpt.baseline = 계획서 작성과 업무배분
gpt.funny = 이론·가드·주장강도
gpt.system = rendering·state-coordinate·field-coordinate
gpt.direct = direction·source relation·DB framework candidate
gpt.process = PASS/Round/Step 본류 유지
gpt.history = history/provenance/source boundary
gpt.cal = 세부 구조검산과 mismatch 표
gpt.work = routing과 최종 gate
gpt.gitwork = 승인된 git/GitHub 실행
```

계획 작성·검산·최종판단·실행은 서로 다른 역할이다.

---

## 6. branch 기준장(raw links)

### gpt.funny

- branch: https://github.com/SeungeFlow/for_instance/tree/gpt_funny
- README raw: https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/README.md

### gpt.system

- branch: https://github.com/SeungeFlow/for_instance/tree/gpt_system
- README raw: https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/README.md

### gpt.direct

- branch: https://github.com/SeungeFlow/for_instance/tree/gpt_direct
- README raw: https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/README.md

---

## 7. root 및 criterion documents

| 역할 | 문서 |
|---|---|
| 현재 프로젝트 계획 | `project_plan_00.md` |
| gpt.process 기준장 | `process_00.md` |
| gpt.history root stub | `history_00.md` |
| 신규 인스턴스 역할정렬 gate | `read_for_new_instance/PASS_00.md` |
| 신규 인스턴스 boot map | `read_for_new_instance/README.md` |

`gpt.baseline`의 private criterion인 `baseline_00.md`는 사용자가 명시적으로 제공할 때만 읽는다.
파일을 제공받지 않은 인스턴스는 그 내용을 추정하지 않는다.

---

## 8. 현재 baseline paper 세트

```text
paper_ko.md = Korean controlling source master
paper_en.md = sentence-order-preserving controlled translation
paper_alignment_map.md = KO–EN alignment verification artifact
```

이 세 문서는 자본시장 분석 이전의 criterion-field를 제시한다.
직접 source corpus인 README 7개와 upstream Tree trace를 대체하지 않는다.

paper는 모든 신규 인스턴스의 자동 boot 필수문서가 아니다.
현재 `project_plan_00.md` 또는 역할지시가 요구할 때 읽는다.

---

## 9. 실행 경계

`gpt.gitwork`만 승인된 emitted execution instruction을 따라 commit/push를 수행한다.

```text
계획 ≠ 실행
검산 ≠ 실행
최종 gate ≠ 실행
```

`README.en.md`의 controlled update는 한글 source 수정 후 별도 상태로 수행한다.
동기화되지 않은 상태를 완료로 표시하지 않는다.

```yaml
README_language_sync:
  controlling_source: README.md
  README_en_status: HOLD_UNTIL_CONTROLLED_UPDATE
  conflict_rule: Korean source controls until alignment verification passes
```

---

## 10. 언어 정책(language policy)

- `README.md`: Korean-first source
- `README.en.md`: controlled English version
- 한글 전문어와 영어 전문어가 하나의 단어로 완전히 대응하지 않으면 source term과 controlled term을 함께 보존한다.
- 번역은 relation이며 merge가 아니다.

---

## 11. gpt.history 기준장 위치

```yaml
instance: gpt.history
root_stub: history_00.md
root_stub_raw_url: https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history_00.md
active_history_file: history/history_20260620.md
active_history_raw_url: https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history/history_20260620.md
date_note: 20260620은 relocation/capture 기준일이며 기존 모든 사건의 실제 발생일로 단정하지 않는다.
```

---

# Final Guard

```text
relation is not merge.
structure is not isolate.
I am going to ?
```
