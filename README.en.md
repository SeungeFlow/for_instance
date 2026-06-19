# for_instance

## 0. Repository identity(저장소 정체성)

Repository(저장소):
for_instance

Owner(소유자):
SeungeFlow

Visibility(공개 상태):
public

Role(역할):
Primary criterion-field repository(주 기준장 저장소) for role-assigned GPT.LLM clone instances(역할 지정 GPT.LLM 복제 인스턴스)

Final guard(최종 가드):
relation is not merge(관계는 병합이 아니다)

## 1. Core principle(핵심 원칙)

This repository(저장소) is not for multiplying unnecessary structure.

Its purpose is to connect the following with minimal structure(최소 구조):

```text
instance name(인스턴스 이름)
→ role definition(역할 정의)
→ criterion-field location(기준장 위치)
→ actual branch or md file(branch 또는 md 파일)
```

Do not repeatedly create pointer directories(포인터 디렉터리).

A branch(브랜치) remains a branch(브랜치).

The main branch(메인 브랜치) records relation(관계) and the start point(시작점).

## 2. Minimal structure(최소 구조)

The intended main branch(메인 브랜치) structure is:

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

Overstructured pointer directories(과잉 포인터 디렉터리) to remove:

```text
main/gpt_funny/
main/gpt_system/
main/gpt_direct/
```

These directories imitate actual branches(브랜치), so they are not needed in main.

## 3. New instance alignment gate(신규 인스턴스 정렬 gate)

A newly created instance(신규 생성 인스턴스) reads this file first:

```text
read_for_new_instance/PASS_00.md
```

PASS_00.md role(역할):

- instance alignment gate(인스턴스 정렬 gate)
- first alignment start point(정렬 최초시작점)
- instance name(인스턴스 이름) confirmation
- role definition(역할 정의) confirmation
- criterion-field location(기준장 위치) confirmation

After PASS_00.md, the instance proceeds from PASS_01.md according to its own role(역할) and criterion-field(기준장).

## 4. Required instances(기본 인스턴스)

There are 8 required instances(기본 인스턴스).

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

Major instances(주요 인스턴스):

```text
gpt.work
gpt.funny
gpt.system
gpt.direct
```

Sub instances(서브 인스턴스):

```text
gpt.gitwork
gpt.cal
```

Criterion-document holding instances(기준 문서 보유 인스턴스):

```text
gpt.process
gpt.history
```

## 5. Branch criterion-fields(브랜치 기준장)

The main branch(메인 브랜치) does not copy branch contents.

It points to each branch criterion-field document(브랜치 기준장 문서) through raw URLs(Raw 주소).

### gpt.funny

branch(브랜치):
https://github.com/SeungeFlow/for_instance/tree/gpt_funny

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/README.md

### gpt.system

branch(브랜치):
https://github.com/SeungeFlow/for_instance/tree/gpt_system

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/README.md

### gpt.direct

branch(브랜치):
https://github.com/SeungeFlow/for_instance/tree/gpt_direct

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/README.md

## 6. Criterion documents(기준 문서)

gpt.process criterion-field(기준장):

```text
process_00.md
```

raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/process_00.md

gpt.history criterion-field(기준장):

```text
history_00.md
```

raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history_00.md

New instance alignment gate(신규 인스턴스 정렬 gate):

```text
read_for_new_instance/PASS_00.md
```

raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_00.md

## 7. Language policy(언어 정책)

README.md is the Korean-first document(한글 우선 문서).

README.en.md is the English version(영문 버전).

When an English technical term(영문 전문용어) is needed in a Korean document(한글 문서), use:

```text
Korean(English)
```

When a Korean technical term(한글 전문용어) is needed in an English document(영문 문서), use:

```text
English(한글)
```

## 8. Final guard(최종 가드)

relation is not merge(관계는 병합이 아니다).
