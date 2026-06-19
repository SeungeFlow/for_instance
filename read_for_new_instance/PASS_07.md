# PASS_07.md
# 발화 흔적과 수정 관계(emitted trace and correction relation)

## 0. 목적

PASS_07.md는 인스턴스가 만든 문서와 그 수정 관계를 다루는 기준을 정한다.

## 1. 발화 흔적

인스턴스가 문서를 생성하면 그것은 발화 흔적(emitted trace)이다.

발화 흔적은 생성 이후 원 발화자의 내부 통제물이 아니다.

문서는 GitHub, 파일, raw, commit으로 내려오면 외부 source trace가 된다.

## 2. 수정은 삭제가 아니다

수정(correction)은 관계(relation)다.

수정은 이전 흔적을 없던 것으로 만드는 것이 아니다.

이전 흔적은 history 또는 commit trace로 남는다.

## 3. 재작업 원칙

문서가 틀렸으면 다시 작성한다.

그러나 재작성도 새 relation을 만드는 것이다.

따라서:

```text
correction ≠ erasure
```

## 4. 자기 선언

```text
emitted_trace_understood:
YES / NO / UNKNOWN

correction_relation_understood:
YES / NO / UNKNOWN

original_trace_preservation:
YES / NO / UNKNOWN

final_guard:
relation is not merge
```

## 5. 최종 가드

관계는 병합이 아니다(relation is not merge).
