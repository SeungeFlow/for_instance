# for_instance

## 0. Repository identity

Repository:
for_instance

Owner:
SeungeFlow

Visibility:
public

Role:
Primary criterion-field repository for role-assigned GPT.LLM clone instances.

Final guard:
relation is not merge.

## 1. Core principle

This repository is not meant to multiply unnecessary structure.

Its purpose is to connect the following in a minimal way:

```text
instance name
→ role definition
→ criterion-field location
→ actual branch or md file
```

Do not repeatedly create pointer directories.

A branch remains a branch.

The main branch records relation and the start point.

## 2. Minimal structure

The intended main branch structure is:

```text
main/
├── README.md
├── README.en.md
├── process_00.md
├── history_00.md
└── read_for_new_instance/
    ├── PASS_00.md
    ├── PASS_01.md
    ├── ...
    └── PASS_10.md
```

Removed overstructured pointer directories:

```text
main/gpt_funny/
main/gpt_system/
main/gpt_direct/
```

Those directories imitated actual branches, so they are not needed in `main`.

## 3. New instance alignment gate

A newly created instance reads this file first:

```text
read_for_new_instance/PASS_00.md
```

`PASS_00.md` is the first alignment gate. It records:

- instance names
- role classes
- role definitions
- criterion-field locations
- source links to branches or md files

After `PASS_00.md`, the instance proceeds from `PASS_01.md` according to its own role and criterion-field.

## 4. Required instances

There are 8 required instances:

```text
gpt.work
gpt.gitwork
gpt.funny
gpt.system
gpt.direct
gpt.cal
gpt.process
gpt.history
```

Major instances:

```text
gpt.work
gpt.funny
gpt.system
gpt.direct
```

Sub instances:

```text
gpt.gitwork
gpt.cal
```

Criterion-document holding instances:

```text
gpt.process
gpt.history
```

## 5. Branch criterion-fields

The main branch does not copy branch contents.

It points to each branch criterion-field document through raw URLs.

### gpt.funny

Branch:
https://github.com/SeungeFlow/for_instance/tree/gpt_funny

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_funny/README.md

### gpt.system

Branch:
https://github.com/SeungeFlow/for_instance/tree/gpt_system

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_system/README.md

### gpt.direct

Branch:
https://github.com/SeungeFlow/for_instance/tree/gpt_direct

README raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/gpt_direct/README.md

## 6. Criterion documents

gpt.process criterion-field:

```text
process_00.md
```

Raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/process_00.md

gpt.history criterion-field:

```text
history_00.md
```

Raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history_00.md

New instance alignment gate:

```text
read_for_new_instance/PASS_00.md
```

Raw:
https://raw.githubusercontent.com/SeungeFlow/for_instance/main/read_for_new_instance/PASS_00.md

## 7. Language policy

`README.md` is the Korean-first document.

`README.en.md` is the English version.

In the Korean-first document, English technical terms may be written as:

```text
Korean(English)
```

In the English version, Korean technical terms may be written as:

```text
English(Korean)
```

The English version should remain English-first. Korean parenthetical terms should be used only when they clarify a SeungeFlow-specific term or an important structural term.

Examples:

- criterion-field(기준장)
- relation(관계)
- merge(병합)
- process(과정)
- history(이력)

## 8. Final guard

relation is not merge.


## gpt.history Criterion Location Update

```yaml
instance: gpt.history
root_stub: history_00.md
root_stub_raw_url: https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history_00.md
active_history_file: history/history_20260620.md
active_history_raw_url: https://raw.githubusercontent.com/SeungeFlow/for_instance/main/history/history_20260620.md
date_note: "20260620 is the relocation/capture date, not necessarily the actual date of every prior event."
final_guard: "relation is not merge"
```

