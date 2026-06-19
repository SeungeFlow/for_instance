# PASS_02.md
# repo/main 읽기 정렬(repo/main reading alignment)

## 0. 목적

PASS_02.md는 신규 인스턴스가 `for_instance` 저장소(repository)의 main 구조를 읽는 단계다.

이 단계에서 인스턴스는 main 브랜치(main branch)가 무엇을 기록하고 무엇을 기록하지 않는지 구분한다.

## 1. 읽을 파일

아래 파일을 읽는다.

```text
README.md
README.en.md
```

기본 기준은 `README.md`다.

`README.md`는 한글 우선 문서(Korean-first document)다.

`README.en.md`는 영문 버전(English version)이다.

## 2. main 브랜치의 역할

main 브랜치(main branch)는 전체 branch 내용을 복사하지 않는다.

main 브랜치는 다음만 기록한다.

1. 저장소 정체성(repository identity)
2. 최소 구조(minimal structure)
3. 신규 인스턴스 시작점(new instance start point)
4. branch Raw 주소(raw URL)
5. process/history 기준문서 위치

## 3. 금지 이해

main 브랜치는 branch를 흉내내는 디렉터리(directory)를 만들지 않는다.

따라서 아래 구조는 사용하지 않는다.

```text
main/gpt_funny/
main/gpt_system/
main/gpt_direct/
```

branch는 branch로 둔다.

관계는 link와 Raw 주소로 기록한다.

## 4. 자기 확인

다음 형식으로 확인한다.

```text
repo:
for_instance

main_read_status:
FULL_READ / PARTIAL_READ / TRUNCATED / SNIPPET_ONLY / UNKNOWN

minimal_structure_understood:
YES / NO / UNKNOWN

final_guard:
relation is not merge
```

## 5. 최종 가드

관계는 병합이 아니다(relation is not merge).
