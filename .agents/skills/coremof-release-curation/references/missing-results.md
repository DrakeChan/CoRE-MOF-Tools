# Unavailable feature and checker results

Start from the requested release's exact IDs, CIF hashes, selected evidence
and attempt records. Missing output alone does not prove that a calculation
was never run or is impossible for that structure.

- Recover valid compatible saved outputs before considering new calculations.
  A downstream model's missing upstream export is not a scientific prediction
  failure. SETC-GAT needs the complete compatible licensed MOSAEC representation
  and atom mapping, not just its verdict or an alternative export.
- Separate resource failures, deterministic tool/input limits, upstream blocks,
  conflicting evidence, confirmed unrun work and unresolved evidence gaps.
  Count unique structures separately from components and attempts.
- Keep intended/expected CIF hash bindings distinct from observed input hashes.
  A worker stopped before reading its CIF need not have an observed hash.
- Check previous attempts and remaining retry limits before an authorized
  same-protocol resource retry. Do not blindly requeue exhausted timeouts or
  deterministic aborts. Exclude legacy zero-probe fields from new/current
  recovery/plots, except where explicitly reproducing a frozen experiment's
  exact historical inputs as a separately labelled result.
- `PeriodicSite.specie` requires an ordered site. Choosing partial/mixed
  occupants, rewriting occupancy, deleting atoms, substituting radii or changing
  the checker/model input contract is not a proven version-only repair.
- Preserve nulls and unavailable statuses. An execution problem is not
  FAIL/NCR. Status-only repairs cannot change votes, scores, labels, features,
  targets, group membership or frozen assignments. A completed FAIL is not
  rerun to obtain PASS.

Restoring an omitted scientific value from selected immutable evidence is an
evidence/projection update, not a status-only repair. Verify a new candidate and
its activation/registration gates, disclose changed coverage or labels and
preserve frozen experiments rather than rewriting their inputs.

Complete the requested saved-evidence recovery and focused checks. New science
outside that scope needs an explicit candidate/method/resource plan and the
user's execution authority. Keep private worker records, recovery inventories
and machine-specific paths outside this portable skill and public packages.
