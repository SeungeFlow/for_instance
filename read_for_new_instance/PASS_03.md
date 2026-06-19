# PASS_03.md
# process/history 경계 확인(process/history boundary)

## 0. 목적

PASS_03.md는 신규 인스턴스가 `process_00.md`와 `history_00.md`의 차이를 이해하는 단계다.

## 1. 읽을 파일

아래 파일을 읽는다.

```text
process_00.md
history_00.md
```

## 2. process_00.md

`process_00.md`는 현재/미래 과정 기준장(current/future process criterion-field)이다.

역할:

1. 공통 가드(common guard)
2. 과정 상속(process inheritance)
3. 신규 인스턴스 시작 순서
4. role boundary
5. no commit / no push boundary

## 3. history_00.md

`history_00.md`는 과거 사건 기록 기준장(past event record criterion-field)이다.

역할:

1. 이미 일어난 사건 기록
2. commit/push 이력 기록
3. 구조 수정 이력 기록
4. correction trace 보존

## 4. 경계

```text
process ≠ history
```

과정(process)은 현재/미래의 기준이다.

이력(history)은 과거 사건의 기록이다.

## 5. 자기 확인

```text
process_00_read_status:
FULL_READ / PARTIAL_READ / TRUNCATED / SNIPPET_ONLY / UNKNOWN

history_00_read_status:
FULL_READ / PARTIAL_READ / TRUNCATED / SNIPPET_ONLY / UNKNOWN

process_history_boundary_understood:
YES / NO / UNKNOWN

final_guard:
relation is not merge
```

## 6. 최종 가드

관계는 병합이 아니다(relation is not merge).
