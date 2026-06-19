# read_for_new_instance

## 0. 디렉터리 정체성(directory identity)

경로(path):
read_for_new_instance/

역할(role):
신규 인스턴스(new instance)의 boot reading sequence를 담는 디렉터리(directory)

최초 gate:
PASS_00.md

최종 가드(final guard):
관계는 병합이 아니다(relation is not merge)

## 1. 읽기 순서(reading order)

신규 인스턴스(new instance)는 다음 순서로 읽는다.

```text
PASS_00.md
→ PASS_01.md
→ PASS_02.md
→ PASS_03.md
→ PASS_04.md
→ PASS_05.md
→ PASS_06.md
→ PASS_07.md
→ PASS_08.md
→ PASS_09.md
→ PASS_10.md
```

PASS_00.md는 인스턴스 정렬 gate(instance alignment gate)다.

PASS_01.md부터 PASS_10.md까지는 PASS_00 이후 실제 자기 역할로 들어가기 위한 boot sequence다.

## 2. 각 PASS의 역할

| 파일(file) | 역할(role) |
|---|---|
| PASS_00.md | 인스턴스 정렬 gate(instance alignment gate) |
| PASS_01.md | 인스턴스 이름 바인딩(instance name binding) |
| PASS_02.md | repo/main 읽기 정렬(repo/main reading alignment) |
| PASS_03.md | process/history 경계 확인(process/history boundary) |
| PASS_04.md | 자기 기준장 바인딩(criterion-field binding) |
| PASS_05.md | source 읽기 상태와 Raw 주소 규칙(source read status and Raw URL discipline) |
| PASS_06.md | 역할 경계와 대체 금지(role boundary and no replacement) |
| PASS_07.md | 발화 흔적과 수정 관계(emitted trace and correction relation) |
| PASS_08.md | 실행 경계와 gpt.gitwork 분리(execution boundary) |
| PASS_09.md | 언어 정책과 출력 규율(language policy and output discipline) |
| PASS_10.md | 최종 자기 선언 gate(final self-declaration gate) |

## 3. 최종 가드(final guard)

관계는 병합이 아니다(relation is not merge).
