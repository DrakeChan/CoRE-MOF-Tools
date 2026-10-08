# Portable benchmark workflow selection

Read only the route needed for the requested experiment:

- **New target-complete benchmark:** use
  [the target-first guide](../../../../docs/source/target_first_benchmark.rst)
  and `examples/build_target_first_benchmark.py`. Attach declared targets,
  determine finite eligibility, then build cohorts. Full-release grouping and
  label purity include target-missing rows. The receipt binds target sources,
  endpoint definitions, eligibility, groups and assignments. Model-input
  certification is a separate step.
- **Frozen paper experiment:** use
  [the replay guide](../../../../docs/source/frozen_assignment_replay.rst)
  and `examples/replay_common_input_benchmark.py`. Verify the supplied archive
  and its assignment receipt. Preserve the recorded checker view, eligibility,
  groups, strata and assignments. A newer dataset is not a replay.
- **General target-independent splitting:** use
  [the splitting handbook](../../../../README_DATASET_SPLITTING.md) and
  [grouped recipes](../../../../examples/grouped_workflow_recipes.md).
  Explicit later attachment preserves the original split digest. A filtered
  `missing="drop"` view never refills, rebalances or resplits.

The [benchmark handoff](../../../../ML_BENCHMARK_HANDOFF.md) describes numerical
requirements and evaluation conventions. The selected handoff's verified
manifest controls exact identities, settings and counts. Preserve earlier
experiments separately, without putting superseded handoff narratives into a
current release guide.

For accepted target aggregation, use
[combined target construction](../../../../COMBINED_TARGET_DATASET.md).
The builder/auditor require an independently pinned identity contract and input
hashes. `examples/extend_collected_targets.py` can extend a compatible target
snapshot using saved evidence while preserving accepted values and scientific
nulls. This is not a new split or a public-release authorization. Coverage comes
from the selected receipt, never completion-only counts or an old guide.
