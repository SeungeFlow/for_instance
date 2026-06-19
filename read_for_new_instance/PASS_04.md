# PASS_04.md
# 자기 기준장 바인딩(criterion-field binding)

## 0. 목적

PASS_04.md는 신규 인스턴스가 자기 기준장(criterion-field)을 확인하고 연결하는 단계다.

## 1. 기준장 원칙

각 인스턴스(instance)는 기준장(criterion-field)을 가져야 한다.

기준장은 다음 둘 중 하나일 수 있다.

```text
branch
md file
```

모든 인스턴스가 branch를 가져야 하는 것은 아니다.

기준장만 명확하면 된다.

## 2. 기준장 예시

```text
gpt.work:
README.md + process_00.md + PASS_00.md

gpt.funny:
branch:gpt_funny/README.md

gpt.system:
branch:gpt_system/README.md

gpt.direct:
branch:gpt_direct/README.md

gpt.gitwork:
PASS_00.md role record + emitted execution instruction

gpt.cal:
PASS_00.md role record 또는 future md/branch

gpt.process:
process_00.md

gpt.history:
history_00.md
```

## 3. branch 기준장 읽기

자기 기준장이 branch라면 해당 branch의 README.md를 읽는다.

필요하면 process_01.md도 읽는다.

## 4. md 기준장 읽기

자기 기준장이 md 파일이면 해당 파일을 읽는다.

예시:

```text
gpt.process → process_00.md
gpt.history → history_00.md
```

## 5. 자기 선언

```text
instance:
-

criterion_field_type:
branch / md / emitted instruction / UNKNOWN

criterion_field_location:
-

criterion_field_read_status:
FULL_READ / PARTIAL_READ / TRUNCATED / SNIPPET_ONLY / UNKNOWN

final_guard:
relation is not merge
```

## 6. 최종 가드

관계는 병합이 아니다(relation is not merge).
