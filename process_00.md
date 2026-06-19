# process_00.md

## 0. 문서 정체성(document identity)

저장소(repository):
for_instance

브랜치(branch):
main

파일(file):
process_00.md

역할(role):
공통 과정 기준장(common process criterion-field)

상태(status):
ROOT_PROCESS_CRITERION_FIELD

최종 가드(final guard):
관계는 병합이 아니다(relation is not merge)

## 1. process_00의 역할

`process_00.md`는 `for_instance` 저장소(repository)의 공통 과정 기준장(common process criterion-field)이다.

각 인스턴스 브랜치(instance branch)의 `process_01.md`는 `process_00.md`를 상속한다.

`process_01.md`는 자기 브랜치의 역할과 세부 과정을 특화할 수 있다.

그러나 `process_01.md`는 `process_00.md`를 대체하지 않는다.

## 2. 공통 가드(common guard)

1. 관계는 병합이 아니다(relation is not merge).
2. 역할(role)은 대체(replacement)가 아니다.
3. 가드(guard)는 사고 수렴 안전장치(thought-convergence safety device)다.
4. `process.md`는 현재/미래 과정 기준장(current/future process field)이다.
5. `history.md`는 과거 사건 기록장(past event record field)이다.
6. 선언(declared)은 검증(verified)이 아니다.
7. 검증(verified)은 수용(accepted)이 아니다.
8. 수용(accepted)은 구현(implemented)이 아니다.
9. 읽기 상태(read status)는 반드시 선언해야 한다.
10. 명시 지시(explicit command) 없이 커밋(commit)하거나 푸시(push)하지 않는다.
11. 브랜치 과정(branch process)은 루트 과정(root process)을 특화할 수 있으나 루트 가드(root guard)를 약화할 수 없다.
12. main 브랜치(main branch)는 관계(relation)를 기록하며, 전체 브랜치 내용(total branch content)을 병합하지 않는다.
13. 주 저장소(primary repo)는 존재할 수 있으나 주 인스턴스(primary instance)는 없다.
14. 발화된 흔적(emitted trace)은 발화자(speaker)의 통제물이 아니다.
15. 수정(correction)은 관계(relation)이지 삭제(erasure)가 아니다.
16. 배치(placement)를 위해서는 source identity가 필요하다.
17. 모르는 값은 반드시 UNKNOWN으로 둔다.

## 3. 인스턴스 과정 상속(instance process inheritance)

각 인스턴스는 자기 기준장(criterion-field)을 가진다.

기준장(criterion-field)은 branch 또는 md 파일일 수 있다.

인스턴스 branch에 `process_01.md`가 있으면 다음 관계를 따른다.

```text
process_00.md
→ process_01.md
```

`process_01.md`는 지역 과정(local process)을 정의한다.

`process_01.md`는 `process_00.md`보다 구체적일 수 있다.

그러나 `process_01.md`는 `process_00.md`의 공통 가드(common guard)를 약화할 수 없다.

## 4. 현재 기본 브랜치(current initial branches)

현재 실제 브랜치(actual branches):

```text
main
gpt_funny
gpt_system
gpt_direct
```

branch는 branch로 둔다.

main 브랜치(main branch)는 branch를 흉내내는 디렉터리(directory)를 만들지 않는다.

branch 관계는 `README.md`와 `read_for_new_instance/PASS_00.md`의 raw 주소(raw URL)로 기록한다.

## 5. 신규 인스턴스 시작 순서(new instance start order)

신규 인스턴스(new instance)는 다음 순서로 시작한다.

1. `read_for_new_instance/PASS_00.md`
2. `README.md` 또는 `README.en.md`
3. `process_00.md`
4. 자기 인스턴스 이름에 해당하는 기준장(criterion-field)
5. 필요한 범위의 `PASS_01.md` 이후 문서
6. 자기 역할 선언(role declaration)
7. 현재 상태 선언(status declaration)

## 6. process와 history의 경계

`process_00.md`는 앞으로 어떻게 진행할지 정의한다.

`history_00.md`는 이미 일어난 일을 기록한다.

따라서:

```text
process ≠ history
```

과정(process)은 미래/현재의 기준이다.

이력(history)은 과거 사건의 기록이다.

## 7. 언어 정책(language policy)

`process_00.md`는 한글 우선 문서(Korean-first document)다.

영문 전문용어(English technical term)가 필요하면 다음 형식을 사용한다.

```text
한글(English)
```

예시:

- 저장소(repository)
- 브랜치(branch)
- 기준장(criterion-field)
- 관계(relation)
- 병합(merge)
- 가드(guard)
- 과정(process)
- 이력(history)
- 커밋(commit)
- 푸시(push)

## 8. 최종 가드(final guard)

관계는 병합이 아니다(relation is not merge).
