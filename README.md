# for_instance

## 0. repo identity

repo:
for_instance

visibility:
public

role:
primary criterion-field repository for role-assigned GPT.LLM clone instances

primary_instance:
NONE

guard:
relation is not merge

## 1. purpose

This repository records the relation field for named GPT instances.

Each instance branch keeps its own criterion-field.

main branch records common process, initial history, reading order, and relation pointers.

## 2. initial branches

- main
- gpt_funny
- gpt_system
- gpt_direct

## 3. branch and pointer rule

branch.gpt_funny is not main/gpt_funny/
branch.gpt_system is not main/gpt_system/
branch.gpt_direct is not main/gpt_direct/

main pointer directories are accepted summary / branch pointer / relation index only.

relation:
YES

merge:
NO
