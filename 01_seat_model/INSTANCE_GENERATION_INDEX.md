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
