# Target-free core metadata and explicit targets

The current layout marker is `target_free_core/1.0`, with individual structural
records `coremof-structure-record/1.2`. Core records/CSV/JSONL contain structural
metadata, features, checker evidence and related groups, not simulation response
values, availability or target-calculation protocols.

Default complete-release and source-projection loading never finds targets
automatically. For an explicitly requested supplement use
`dataset.attach_target_supplement(root, expected_sha256=trusted_manifest_hash)`.
The supplement `coremof-target-supplement/1.0` binds the exact core input hashes,
IDs, CSV/JSONL, units and endpoint conditions. Only the three response values
are joined. Statuses, native nulls, methods and full observation provenance stay
in the separate package. Preserve zeros. Do not impute, clip, refill or resplit.

Historical combined inputs remain immutable. Explicit
`include_legacy_targets=True` is available for historical reproduction only.
It does not bypass the target-free marker's purity checks or admission gates.
Source hashes describe original file bytes, not the sanitized default view.

A packaging/status-reporting revision does not authorize new scientific
calculations or change checker votes, structural values, frozen assignments,
source permissions or release-admission conditions. An unavailable execution
is not FAIL. Resolve recoverable execution causes using existing raw evidence.
Choosing occupants, rewriting disorder or modifying a checker input contract
requires a separately defined method and does not silently repair an old result.
Use [missing-results.md](missing-results.md) to distinguish missing exports,
recorded failures and confirmed unrun tasks. Preserve the repository's existing
ID/path admission rules when importing schemas. Verify the relevant default
load and explicit attachment behavior, and report optional test dependencies
that could not be exercised rather than claiming full backend validation.

See `docs/source/target_supplements.rst` and
`examples/attach_target_supplement.py` in the repository root for usage.
