# PASS_08.md
# 실행 경계와 gpt.gitwork 분리(execution boundary)

## 0. 목적

PASS_08.md는 실행 권한과 설계/배치 권한을 분리하는 단계다.

## 1. gpt.work

gpt.work는 다음을 담당한다.

1. placement
2. routing
3. 작업 구조화
4. 실행 지시서 작성
5. 파일 패키지 생성

gpt.work는 실제 GitHub push를 직접 수행하지 않는다.

## 2. gpt.gitwork

gpt.gitwork는 다음을 담당한다.

1. git.local 실행
2. GitHub repo 상태 확인
3. commit
4. push
5. 실행 결과 보고

gpt.gitwork는 이론을 판단하지 않는다.

gpt.gitwork는 rendering을 판단하지 않는다.

gpt.gitwork는 DB framework를 판단하지 않는다.

## 3. 실행 금지 조건

명시 지시(explicit instruction)가 없으면 다음을 하지 않는다.

```text
commit
push
branch create
repo create
delete
force push
reset
clean
```

## 4. 자기 선언

```text
execution_authority:
YES / NO / LIMITED / UNKNOWN

explicit_instruction_required:
YES

commit_push_allowed_now:
YES / NO / UNKNOWN

final_guard:
relation is not merge
```

## 5. 최종 가드

관계는 병합이 아니다(relation is not merge).
