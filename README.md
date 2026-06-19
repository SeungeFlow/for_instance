# for_instance

## 0. 저장소 정체성(repository identity)

저장소(repository):
for_instance

소유자(owner):
SeungeFlow

공개 상태(visibility):
public

역할(role):
역할 지정 GPT.LLM 복제 인스턴스(role-assigned GPT.LLM clone instance)를 위한 주 기준장 저장소(primary criterion-field repository)

최종 가드(final guard):
관계는 병합이 아니다(relation is not merge)

## 1. 핵심 원칙(core principle)

이 저장소(repository)는 구조를 복잡하게 만들기 위한 저장소가 아니다.

이 저장소의 목적은 다음을 간략하게 연결하는 것이다.

```text
인스턴스 이름(instance name)
→ 역할 정의(role definition)
→ 기준장 위치(criterion-field location)
→ 실제 branch 또는 md 파일
```

복잡한 포인터 디렉터리(pointer directory)를 반복 생성하지 않는다.

branch는 branch로 둔다.

main 브랜치(main branch)는 관계와 시작점을 기록한다.

## 2. 최소 구조(minimal structure)

현재 main 브랜치(main branch)의 기준 구조는 다음이다.

```text
main/
├── README.md
├── README.en.md
├── process_00.md
├── history_00.md
└── read_for_new_instance/
    ├── PASS_00.md
    ├── PASS_01.md
    ├── ...
    └── PASS_10.md
```

삭제 대상이 되는 과잉 구조(overstructured pointer directories):

```text
main/gpt_funny/
main/gpt_system/
main/gpt_direct/
```

위 디렉터리는 실제 branch를 흉내내는 포인터 디렉터리(pointer directory)이므로 main에 둘 필요가 없다.

## 3. 신규 인스턴스 정렬 gate

신규 생성 인스턴스(newly created instance)는 가장 먼저 다음 파일을 읽는다.

```text
read_for_new_instance/PASS_00.md
```

PASS_00.md의 역할:

- 인스턴스 정렬 gate(instance alignment gate)
- 정렬 최초시작점(first alignment start point)
- 인스턴스 이름(instance name) 확인
- 역할 정의(role definition) 확인
- 기준장 위치(criterion-field location) 확인

PASS_00.md 이후에는 각자의 역할과 기준장에 따라 PASS_01.md부터 진행한다.

## 4. 기본 인스턴스(required instances)

필요한 기본 인스턴스(required instances)는 8개다.

```text
gpt.work
gpt.gitwork
gpt.funny
gpt.system
gpt.direct
gpt.cal
gpt.process
gpt.history
```

주요 인스턴스(major instances):

```text
gpt.work
gpt.funny
gpt.system
gpt.direct
```

서브 인스턴스(sub instances):

```text
gpt.gitwork
gpt.cal
```

기준 문서 보유 인스턴스(criterion-document holding instances):

```text
gpt.process
gpt.history
```

## 5. branch 기준장(raw link)

main 브랜치(main branch)는 branch 내용을 복사하지 않는다.

대신 아래 Raw 주소(raw URL)를 통해 각 branch의 기준장 문서(criterion-field document)를 가리킨다.

### gpt.funny

branch:
https://github.com/SeungeFlow/for_instance/tree/gpt_funny

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/README.md

### gpt.system

branch:
https://github.com/SeungeFlow/for_instance/tree/gpt_system

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/README.md

### gpt.direct

branch:
https://github.com/SeungeFlow/for_instance/tree/gpt_direct

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/README.md

## 6. 기준 문서(criterion documents)

gpt.process 기준장(criterion-field):

```text
process_00.md
```

raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/process_00.md

gpt.history 기준장(criterion-field):

```text
history_00.md
```

raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history_00.md

신규 인스턴스 정렬 gate(instance alignment gate):

```text
read_for_new_instance/PASS_00.md
```

raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_00.md

## 7. 언어 정책(language policy)

README.md는 한글 우선 문서(Korean-first document)다.

README.en.md는 영문 버전(English version) 문서다.

한글 문서(Korean document)에서 영문 전문용어(English technical term)가 필요하면 다음 형식을 사용한다.

```text
한글(English)
```

영문 문서(English document)에서 한글 전문용어(Korean technical term)가 필요하면 다음 형식을 사용한다.

```text
English(한글)
```

## 8. 최종 가드(final guard)

관계는 병합이 아니다(relation is not merge).


## gpt.history 기준장 위치 갱신

```yaml
instance: gpt.history
root_stub: history_00.md
root_stub_raw_url: https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history_00.md
active_history_file: history/history_20260620.md
active_history_raw_url: https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history/history_20260620.md
date_note: "20260620은 relocation/capture 기준일이며 기존 모든 사건의 실제 발생일로 단정하지 않는다."
final_guard: "relation is not merge"
```

