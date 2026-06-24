# PASS_10 한글–영문 대응검산 지도

- **검산 상태:** `PASS`
- **진행 회차:** `PASS_10`
- **사용 모드:** `Pro.확장`

- **게시용 파일명:** `paper_alignment_map.md`
- **원 생성 파일명:** `PASS_10_KO_EN_ALIGNMENT_MAP.md`
- **한글 원본:** `paper_ko.md`
- **영문 통제번역:** `paper_en.md`
- **한글 SHA-256:** `772d6dbe5c2bd73637edfe33197d657aab83032c48938d7c80b5c261c977e253`
- **영문 SHA-256:** `005e2279584212bfcc6f68624a6976cbe568220150ecf42a8787f8f427eb432c`

## 1. 검산 원칙

- 한글본이 의미·주장강도·미확정 상태를 통제하는 원본이다.
- 영문본은 독립 재서술이 아니라 section·paragraph 순서를 보존한 통제번역이다.
- 영문본에 새로운 주장, 예시, 외부증거 또는 결론을 추가하지 않는다.
- `CS`, `RS`, `SI`, `PC`와 `HOLD`, `UNKNOWN`, `CANDIDATE`, `VERIFIED_WITHIN_SCOPE`의 경계를 보존한다.

## 2. Section 대응

| 한글 원본 | 영문 통제번역 | 상태 |
|---|---|---|
| 초록 | Abstract | 대응 완료 |
| 1. 서론: 분석결과보다 먼저 필요한 기준 | 1. Introduction: Criteria Needed Before Analytical Results | 대응 완료 |
| 2. 자료와 방법: 경계를 보존한 공통구조 추출 | 2. Materials and Method: Extracting Common Structure While Preserving Boundaries | 대응 완료 |
| 3. 결과: 자본시장 분석 이전의 공통 기준 | 3. Results: Common Criteria Before Capital-Market Analysis | 대응 완료 |
| 4. 일곱 인스턴스의 역할관계 | 4. Role Relations Among the Seven Instances | 대응 완료 |
| 5. 인간과 인공지능이 함께 읽는 게시구조 | 5. Publication Structure Readable by Humans and AI | 대응 완료 |
| 6. 한계와 현재 상태 | 6. Limitations and Current Status | 대응 완료 |
| 7. 결론: 다음 분석을 열기 위한 기준장 | 7. Conclusion: A Criterion-Field That Opens the Next Analysis | 대응 완료 |
| 부록 A. Source key와 claim–source relation map | Appendix A. Source Keys and Claim–Source Relation Map | 대응 완료 |
| 부록 B. 한글–영문 통제 용어표 | Appendix B. Korean–English Controlled Terminology Table | 대응 완료 |

## 3. 구조검산 결과

| 검산항목 | 결과 |
|---|---|
| `korean_master_exists` | `PASS` |
| `english_translation_exists` | `PASS` |
| `title_locked_in_both` | `PASS` |
| `claim_id_sets_identical` | `PASS` |
| `all_seven_sources_in_both` | `PASS` |
| `guard_relation_preserved` | `PASS` |
| `guard_structure_preserved` | `PASS` |
| `status_hold_preserved` | `PASS` |
| `status_unknown_preserved` | `PASS` |
| `status_candidate_preserved` | `PASS` |
| `status_verified_within_scope_preserved` | `PASS` |
| `fenced_block_count_equal` | `PASS` |
| `table_row_count_equal` | `PASS` |
| `numbered_sections_equal` | `PASS` |
| `numbered_subsections_equal` | `PASS` |
| `appendices_present` | `PASS` |
| `english_alignment_markers_present` | `PASS` |
| `publication_not_falsely_marked_complete` | `PASS` |

## 4. 정량 대응값

- Claim relation ID: 한글 `20`개 / 영문 `20`개 / 차이 `0`개
- Claim relation ID 목록: `CS-01, CS-02, CS-03, CS-04, CS-05, CS-06, CS-07, PC-01, PC-02, PC-03, RS-CAL, RS-DIR, RS-FNY, RS-HIS, RS-PRO, RS-SYS, RS-WRK, SI-01, SI-02, SI-03`
- Fenced code delimiter: 한글 `12` / 영문 `12`
- Markdown table row: 한글 `81` / 영문 `81`
- 영문 alignment marker: `46`개

## 5. 통제번역 판정

- 제목, 제목에 해당하는 압축문장, 초록, 본문 7개 절, 부록 A·B가 대응한다.
- 7개 README source key와 claim–source relation은 동일하게 유지되었다.
- 두 중심 가드와 미확정 상태값이 영문본에서도 유지되었다.
- 한글본에 포함된 `Controlled English Abstract`는 별도 논문이 아니라 요약 대응부이며, 영문 전체본의 Abstract와 같은 주장범위를 가진다.
- 실제 GitHub source freeze, 외부 인용 조립, 실증검증과 논문게시는 아직 실행되지 않았다.

> relation is not merge, structure is not isolate.
