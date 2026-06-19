# read_for_new_instance

## role

This directory contains the boot reading sequence for future named GPT instances.

New instances read:

1. main/README.md or main/README.en.md
2. main/process_00.md
3. read_for_new_instance/PASS_01.md through PASS_10.md
4. assigned branch/process_01.md
5. assigned branch files
6. self-declaration

guard:
relation is not merge
