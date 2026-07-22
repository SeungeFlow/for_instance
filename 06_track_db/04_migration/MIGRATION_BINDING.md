---
document_type: HRTDB_A_TRACK_DB_PHASE2A_MIGRATION_BINDING
---

# HRTDB_A Track DB Phase 2A Migration Binding

```yaml
migration:
  source_repository_seat: B
  source_repository: LRSDoNet_B
  source_repository_id: 1300913958
  source_ref: TrackDB
  source_head: de0a6e1f6435ef78e5b95f02f8bd5b8d5459d3f1
  source_tree: c822f3a644bb58f29ddbf262a3f727a3da3cbdcc

  target_repository_seat: A
  target_repository: HRTDB_A
  target_repository_id: 1300938880
  target_ref: TrackDB
  target_parent: e696776a4715b46fa68e3e3af55f860835f80b1c
  target_head_after: EXTERNAL_PHASE2A_CLOSURE
  target_tree_after: EXTERNAL_PHASE2A_CLOSURE

  phase1_evidence_bundle:
    filename: f5c6610ae834143307b2502b517d395612a01851ceeedb614ad804fbc7d95009.zip
    sha256: f5c6610ae834143307b2502b517d395612a01851ceeedb614ad804fbc7d95009
    verdict: PASS_TRACK_DB_MIGRATION_CANDIDATES_CLASSIFIED
    candidate_count: 25

  phase1_move_ref_observation_count: 14
  authorized_trackdb_move_object_count: 11
  skipped_duplicate_ref_observation_count: 3
  copied_exact_object_count: 4
  updated_revision_count: 7
  pointer_only_count: 0
  no_move_count: 11
  source_removed: false
```

## Self-reference boundary

동일한 단일 Commit 내부 문서에 그 Commit 자신의 최종 SHA와 Tree를
실제값으로 포함할 수 없으므로, `target_head_after`와
`target_tree_after`는 외부 Phase 2A Closure Bundle에서 결속한다.

```text
Copy precedes source removal.
Target readback precedes migration closure.
Original Registration Event is not Migration Event.
relation is not merge.
relation is interconnecting.
```
