# PASS_05.md
# source 읽기 상태와 Raw 주소 규칙(source read status and Raw URL discipline)

## 0. 목적

PASS_05.md는 신규 인스턴스가 source를 읽었다고 주장할 때 그 읽기 상태를 정확히 선언하게 하는 단계다.

## 1. 읽기 상태 값

허용되는 read_status 값은 다음이다.

```text
FULL_READ
PARTIAL_READ
TRUNCATED
SNIPPET_ONLY
UNKNOWN
```

## 2. 값은 값이다

읽지 않은 것을 읽었다고 말하지 않는다.

일부만 본 경우 `PARTIAL_READ` 또는 `TRUNCATED`로 선언한다.

요약만 본 경우 `SNIPPET_ONLY`로 선언한다.

모르면 `UNKNOWN`으로 둔다.

## 3. Raw 주소 규칙

GitHub 문서를 기준으로 삼을 때는 가능하면 Raw 주소(raw URL)를 함께 기록한다.

예시:

```text
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/README.md
```

Raw 주소는 사람이 보는 GitHub HTML 화면보다 기준문서 내용을 직접 읽는 데 적합하다.

## 4. 자기 선언

```text
source:
-

raw_url:
-

read_status:
FULL_READ / PARTIAL_READ / TRUNCATED / SNIPPET_ONLY / UNKNOWN

source_identity_preserved:
YES / NO / UNKNOWN

final_guard:
relation is not merge
```

## 5. HOLD 조건

아래 경우 HOLD 한다.

- source 위치가 없음
- Raw 주소가 필요한데 없음
- 읽기 상태를 알 수 없음
- source를 읽지 않고 FULL_READ라고 주장하려 함

## 6. 최종 가드

관계는 병합이 아니다(relation is not merge).
