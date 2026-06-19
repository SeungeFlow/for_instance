# PASS_09.md
# 언어 정책과 출력 규율(language policy and output discipline)

## 0. 목적

PASS_09.md는 문서 언어 정책과 출력 규율을 정한다.

## 1. 기본 언어 정책

기본 문서가 `README.md`, `process_00.md`, `history_00.md`, `PASS_00.md` 계열이면 한글 우선 문서(Korean-first document)를 기본으로 한다.

영문 버전이 필요하면 `.en.md` 파일로 분리한다.

## 2. 병용 표기

한글 문서에서 영문 전문용어가 필요하면 다음 형식을 사용한다.

```text
한글(English)
```

영문 문서에서 한글 전문용어가 필요하면 다음 형식을 사용한다.

```text
English(한글)
```

단, 영문 문서에서는 한국어 병기를 과도하게 반복하지 않는다.

## 3. 구조 출력 규율

복잡한 구조보다 간략한 구조를 우선한다.

새 파일을 만들기 전에 기존 구조 안에서 수용할 위치를 먼저 찾는다.

새 디렉터리를 만들기 전에 branch, md 파일, Raw 주소로 충분한지 확인한다.

## 4. 자기 선언

```text
language_policy_understood:
YES / NO / UNKNOWN

minimal_structure_understood:
YES / NO / UNKNOWN

output_discipline_understood:
YES / NO / UNKNOWN

final_guard:
relation is not merge
```

## 5. 최종 가드

관계는 병합이 아니다(relation is not merge).
