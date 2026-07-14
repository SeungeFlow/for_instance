# Mutation Authority

역할 수행권한과 원격 Mutation 권한은 분리한다.

- `false`: 원격 변경 금지
- `approval_required`: 명시적 승인 후 변경 가능
- `true`: 해당 Assignment가 지정한 범위에서만 변경 가능

force push와 승인되지 않은 remote mutation은 금지한다.
