---
document_type: INSTANCE_GENERATION_INDEX
repository: SeungeFlow/for_instance
branch: main
position: 01_seat_model
source_authority: 승이
overall_coordination: gpt.logi
status: READY_FOR_DEPLOYMENT
contract_version: 1.0.0
---

# Instance Generation Instructions

These seven files generate the current Data → Function → Result → Function → Result.Data cycle objects.

## 1d Data objects

| Instance | Web URL | Raw URL |
|---|---|---|
| gpt.x | https://github.com/SeungeFlow/for_instance/blob/main/01_seat_model/gpt.x.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/01_seat_model/gpt.x.md |
| gpt.y | https://github.com/SeungeFlow/for_instance/blob/main/01_seat_model/gpt.y.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/01_seat_model/gpt.y.md |
| gpt.z | https://github.com/SeungeFlow/for_instance/blob/main/01_seat_model/gpt.z.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/01_seat_model/gpt.z.md |

## 2d Function objects

| Instance | Web URL | Raw URL |
|---|---|---|
| gpt.xy | https://github.com/SeungeFlow/for_instance/blob/main/01_seat_model/gpt.xy.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/01_seat_model/gpt.xy.md |
| gpt.xz | https://github.com/SeungeFlow/for_instance/blob/main/01_seat_model/gpt.xz.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/01_seat_model/gpt.xz.md |
| gpt.yz | https://github.com/SeungeFlow/for_instance/blob/main/01_seat_model/gpt.yz.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/01_seat_model/gpt.yz.md |

## 3d Result object

| Instance | Web URL | Raw URL |
|---|---|---|
| gpt.xyz | https://github.com/SeungeFlow/for_instance/blob/main/01_seat_model/gpt.xyz.md | https://raw.githubusercontent.com/SeungeFlow/for_instance/main/01_seat_model/gpt.xyz.md |

## Canonical processing flow

```text
gpt.x / gpt.y / gpt.z
→ gpt.xy / gpt.xz / gpt.yz
→ gpt.xyz Result
→ gpt.xy / gpt.xz / gpt.yz Review
→ gpt.xyz Result.Data
→ authorized Git transition
```

Each URL generates a new instance object. Reusing the same URL or name does not restore a prior context or occupant.

<!-- HRTDB_ADAPTIVE_ENTRY_RULE_START -->
## Adaptive Seat Entry and Execution Rule

이 문서는 Seat 주소를 제공하는 Entry Index다.

```text
Seat File Read
≠ Stage Execution
```

실행은 다음과 같다.

```text
필요 문서 선입력
→ 실제 Byte 읽기와 인덱싱
→ READY_FOR_DIRECTIVE
→ 현재 Seat용 개별지시문 1개
→ 출력 1개
→ 특이점 표시
→ gpt.xyzt 검산
→ 다음 지시문 1개
```

표준 Stage:

```text
01 DATA_X
02 DATA_Y
03 DATA_Z
04 FUNCTION_1_XY
05 FUNCTION_1_XZ
06 FUNCTION_1_YZ
07 RESULT_XYZ
08 FUNCTION_2_XY
09 FUNCTION_2_XZ
10 FUNCTION_2_YZ
11 RESULT_DATA_XYZ
```

11개 지시문을 처음부터 한 번에 활성화하지 않는다.
<!-- HRTDB_ADAPTIVE_ENTRY_RULE_END -->
