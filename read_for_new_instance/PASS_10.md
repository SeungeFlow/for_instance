# PASS_10.md
# 최종 자기 선언 gate(final self-declaration gate)

## 0. 목적

PASS_10.md는 신규 인스턴스가 작업을 시작하기 전에 자기 상태를 최종 선언하는 gate다.

## 1. 시작 조건

인스턴스는 다음을 확인한 뒤 시작한다.

1. PASS_00.md를 읽었다.
2. 자기 이름을 확인했다.
3. main README를 읽었다.
4. process_00.md와 history_00.md의 경계를 이해했다.
5. 자기 기준장(criterion-field)을 확인했다.
6. source 읽기 상태(read status)를 선언했다.
7. 역할 경계(role boundary)를 이해했다.
8. 실행 권한(execution authority)을 확인했다.
9. 언어 정책(language policy)을 이해했다.
10. 최종 가드(final guard)를 보존했다.

## 2. 최종 선언 형식

아래 형식으로 선언한다.

```text
instance:
-

class:
major / sub / criterion holder / UNKNOWN

role:
-

criterion_field:
-

read_files:
-

read_status:
FULL_READ / PARTIAL_READ / TRUNCATED / SNIPPET_ONLY / UNKNOWN

role_boundary:
CLEAR / UNCLEAR / UNKNOWN

execution_authority:
YES / NO / LIMITED / UNKNOWN

current_status:
READY / HOLD

hold_reason:
-

final_guard:
relation is not merge
```

## 3. READY 조건

다음이 모두 충족되면 READY다.

```text
instance known
role known
criterion field known
read status declared
role boundary clear
final guard preserved
```

## 4. HOLD 조건

다음 중 하나라도 해당하면 HOLD다.

```text
instance unknown
role unknown
criterion field unknown
source unread but claimed as read
role boundary unclear
execution authority unclear
final guard not preserved
```

## 5. 최종 가드

관계는 병합이 아니다(relation is not merge).
