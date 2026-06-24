# read_for_new_instance

## 0. 디렉터리 정체성(directory identity)

```yaml
path: read_for_new_instance/
role: boot reading sequence for newly created role-assigned instances
first_gate: PASS_00.md
current_plan: ../project_plan_00.md
```

이 디렉터리는 신규 인스턴스가 자신의 이름·역할·기준장·현재 계획을 확인하고 자기 역할로 진입하기 위한 boot sequence를 담는다.

---

## 1. 진입층과 boot gate의 구분

저장소를 통해 들어오는 경우의 진입층:

```text
../README.md
>>> README.md
>>> PASS_00.md
```

- `../README.md`: repository identity와 전체 시작점
- 이 `README.md`: boot map
- `PASS_00.md`: boot sequence의 최초 역할정렬 gate

따라서 root README와 directory README는 위치를 찾는 진입문서이며, `PASS_00.md`는 역할을 고정하는 최초 gate다.

직접 `PASS_00.md`를 받은 인스턴스는 PASS_00의 지시에 따라 두 README와 현재 계획의 read status를 확인한다.

---

## 2. boot reading order

```text
PASS_00.md
>>> project_plan_00.md
>>> PASS_01.md
>>> PASS_02.md
>>> PASS_03.md
>>> PASS_04.md
>>> PASS_05.md
>>> PASS_06.md
>>> PASS_07.md
>>> PASS_08.md
>>> PASS_09.md
>>> PASS_10.md
```

`project_plan_00.md`는 PASS numbering에 포함되지 않는다.
현재 작업의 방향·phase·HOLD·업무배분을 제공하는 operating plan이다.

PASS_01부터 PASS_10까지는 PASS_00 이후 실제 자기 역할로 들어가기 위한 boot sequence다.

---

## 3. 각 PASS의 역할

| 파일 | 역할 |
|---|---|
| `PASS_00.md` | instance alignment gate / 역할·기준장·현재 계획 확인 |
| `PASS_01.md` | instance name binding |
| `PASS_02.md` | repo/main reading alignment |
| `PASS_03.md` | process/history boundary |
| `PASS_04.md` | criterion-field binding |
| `PASS_05.md` | source read status and Raw URL discipline |
| `PASS_06.md` | role boundary and no replacement |
| `PASS_07.md` | emitted trace and correction relation |
| `PASS_08.md` | execution boundary and gpt.gitwork separation |
| `PASS_09.md` | language policy and output discipline |
| `PASS_10.md` | final self-declaration gate |

---

## 4. 계획 우선 규칙

신규 인스턴스는 계획 없이 source를 대규모로 펼치거나 구현을 시작하지 않는다.

```text
현재 계획 확인
>>> 자기 역할 확인
>>> 할당된 source만 읽기
>>> read status 선언
>>> 산출물 생성
>>> 구조검산
>>> handoff
```

`L7OS_for_M7DQ.zip`, rendering branch, 대규모 Tree 문서묶음은 현재 계획이 지정한 범위만 읽는다.
전체 source를 한 회차에 펼치지 않는다.

---

## 5. paper 세트 읽기 규칙

현재 paper 세트:

```text
../paper_ko.md
../paper_en.md
../paper_alignment_map.md
```

관계:

```text
paper_ko.md = controlling source master
paper_en.md = controlled translation projection
paper_alignment_map.md = alignment verification artifact
```

paper는 README 7개와 upstream Tree trace의 전체 source를 대체하지 않는다.

모든 신규 인스턴스가 자동으로 paper 전체를 읽는 것은 아니다.
현재 plan 또는 역할지시가 요구하는 경우에 읽고, 다음 중 하나로 상태를 선언한다.

```text
FULL_READ
PARTIAL_READ
TRUNCATED
SNIPPET_ONLY
UNKNOWN
```

---

## 6. 문맥 과확장 방지

- Library 또는 긴 md가 전체 로드되었다고 가정하지 않는다.
- summary를 source 전체로 취급하지 않는다.
- source identity와 projection을 분리한다.
- `///`는 문맥 구분자로 읽는다.
- `>>>`는 방향기호 `→`로 읽는다.
- 단독 `>`는 수학연산자 가능성을 보존한다.

### 6.1 언어 source 우선순위

root `README.md`와 `README.en.md`의 내용이 아직 동기화되지 않았다면 한글 `README.md`를 controlling source로 읽는다.
영문본의 최신 정렬을 추정하지 않고 read status와 alignment status를 선언한다.

---

## 7. 실행 경계

신규 인스턴스는 승인 없이 commit/push를 수행하지 않는다.
실행은 `gpt.gitwork`의 역할이다.

```text
analysis output
>>> verification
>>> gpt.work final gate
>>> emitted execution instruction
>>> gpt.gitwork execution
```

---

# Final Guard

```text
relation is not merge.
structure is not isolate.
I am going to ?
```
