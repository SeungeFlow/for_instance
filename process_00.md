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

## 9. 대규모 작업 분절 규정(Project Block / Round / PASS / Step-Check)

### 9.0 문서 지위

`process_00.md`는 SeungeFlow 계정 전체 인스턴스가 공통으로 따르는 root process criterion-field이다.

각 branch 또는 인스턴스의 세부 process 문서는 `process_00.md`를 상속할 수 있으나, 이를 대체하거나 약화할 수 없다.

### 9.1 boot PASS와 operation PASS 구분

`read_for_new_instance/PASS_00.md`부터 `PASS_10.md`까지는 신규 인스턴스 정렬 gate이다.

본 장의 `PASS_NN`은 정렬 이후 작업계획, 협의, 실행요청, 검증, 이력 기록을 위한 operation PASS이다.

두 PASS 체계는 관계를 가지지만 병합되지 않는다.

### 9.2 작업 계층

대규모 작업은 다음 계층으로 분절한다.

- Project Block: 하나의 큰 목표를 실제로 다룰 수 있게 끊은 작업 묶음
- Round: Project Block 내부의 중간 검산 단위
- PASS: Round 내부의 guarded work-cycle
- Step / Check: PASS 내부의 최소 수행·확인 단위

### 9.3 상한 규정

하나의 Project Block은 표준적으로 30 PASS 안에서 닫는다.

명시적 council 승인과 재계획이 있을 때만 최대 70 PASS 이하까지 예외 확장할 수 있다.

다음은 금지한다.

- PASS_100
- PASS_200
- 무한 PASS 증가
- 목표 재확인 없는 회차 연장
- Round closure 없는 PASS 누적

Round는 기본 5 PASS 안에서 닫고, 예외적으로 7 PASS를 초과하기 전 재검산한다.

하나의 PASS 안의 Step / Check는 10개를 넘기지 않는다.

### 9.4 closure 규정

Round closure 전에는 다음 Round로 이동할 수 없다.

Project Block closure 전에는 다음 Project Block으로 이동할 수 없다.

GitHub 변경이 발생한 PASS는 Raw URL 검증과 history 기록이 완료되기 전까지 CLOSED로 선언할 수 없다.

### 9.5 실행 경로

외부 기억장 GitHub로 나가는 모든 실행은 다음 경로를 따른다.

`primary council → gpt.work → gpt.gitwork → GitHub → Raw URL verification → gpt.history`

다음 경로는 금지한다.

`primary instance → gpt.gitwork 직접 접속`

`branch instance → gpt.gitwork 직접 접속`

`context.window → gpt.gitwork 직접 접속`

### 9.6 HOLD 조건

다음 조건이 발생하면 작업은 HOLD로 전환한다.

- source identity가 UNKNOWN인 경우
- read_status가 UNKNOWN인데 읽었다고 주장하는 경우
- role boundary가 불명확한 경우
- gpt.work 없이 gpt.gitwork 직접 접속을 시도한 경우
- Project Block 상한을 초과한 경우
- Round closure 없이 PASS만 증가한 경우
- Raw URL 검증 전 완료를 선언한 경우
- GitHub 변경 후 history 기록이 누락된 경우
- process와 history를 혼동한 경우
- relation을 merge로 처리한 경우

### 9.7 Raw URL 읽기 및 source identity 기록 규칙

GitHub 문서를 읽거나 검증할 때는 GitHub 화면 주소와 Raw 주소를 구분한다.

GitHub 화면 주소는 사람이 보는 주소이고, Raw 주소는 인스턴스가 실제로 읽는 원문 주소이다.

앞으로 생성되는 md 문서는 가능한 경우 다음 source identity를 기록한다.

```yaml
instance: process_00
source_identity_required:
  repo: "<OWNER>/<REPO>"
  branch: "<BRANCH>"
  path: "<PATH>"
  github_blob_url: "https://github.com/<OWNER>/<REPO>/blob/<BRANCH>/<PATH>"
  raw_url: "https://raw.githubusercontent.com/<OWNER>/<REPO>/refs/heads/<BRANCH>/<PATH>"
  commit_sha: "<검증 시점의 commit SHA 또는 UNKNOWN>"
  commit_pinned_raw_url: "https://raw.githubusercontent.com/<OWNER>/<REPO>/<COMMIT_SHA>/<PATH>"
```

branch Raw URL은 최신 branch 상태를 따라가므로 나중에 내용이 바뀔 수 있다.

검증 시점의 원문을 고정해야 하는 경우 commit SHA가 들어간 commit-pinned Raw URL을 함께 기록한다.

GitHub 화면 주소와 Raw 주소가 다르게 보이면 Raw 주소를 우선 기준으로 삼는다.

Raw 읽기 실패, commit SHA 미확인, branch/path 불일치가 발생하면 read_status를 UNKNOWN 또는 HOLD로 선언한다.

### 9.8 block 표시 규정

`process_00.md`에 표시되는 모든 code block, yaml block, json block, pseudocode block, structured block 내부에는 반드시 `instance` 필드를 둔다.

기본값은 다음과 같다.

```yaml
instance: process_00
```

### 9.9 final guard

관계는 병합이 아니다.

`relation is not merge`

