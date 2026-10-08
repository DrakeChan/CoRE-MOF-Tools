---
name: coremof-release-curation
description: Read saved CoRE-MOF-COD checker results or prepare and replay grouped CR/NCR benchmarks from an explicitly versioned release.
---

# CoRE-MOF-COD dataset workflows

Use this portable skill for saved release evidence and grouped benchmark data.
It does not contain scheduler instructions or authorize new scientific runs.

## Read only what the task needs

- For metadata or recorded checker outcomes, use `examples/read_release_metadata.py`
  or `examples/read_checker_results.py` and the [database access guide](../../../README_DATABASE_ACCESS.md).
  Reading saved results requires no checker engine or CCDC installation.
- For explicit target attachment or core-export validation, read
  [target separation](references/target-separation.md). Core metadata is
  target-free. A target package beside it is not permission to load it.
- For missing feature/checker results, read
  [missing results](references/missing-results.md). An absent output does not
  prove that the calculation was unrun or scientifically impossible.
- For a new benchmark or frozen replay, read
  [workflow selection](references/dataset-splitting-ml-benchmark.md).
  Use the supplied experiment manifest, not another guide's counts or seeds.

## Identity and scientific boundaries

Use **CoRE-MOF-COD**. CoRE IDs have the form
`YYYY[elements][topology]dimension[variant]serial`. Use `CoREMOF.parse_core_id`
and obtain source/access categories from metadata, not filenames. CoRE IDs are
not chemical MOFid-v1/v2 strings. Descriptive name tokens are not grouping
criteria. Established IDs are persistent by default. Updating an unavailable
`[nan]` topology requires explicit user approval, a validated unambiguous
CrystalNets SingleNodes result and a collision-free registry allocation.
Parsing or formatting does not authorize renaming. Keep retired-ID crosswalks
private. Replaying translated experiments preserves membership and partitions
without resampling newly sorted identifiers.

CR requires all selected checker votes PASS, NCR all FAIL. A complete mixture
is AMBIGUOUS, and an unavailable vote yields UNCHECKED. Execution failures are
not FAIL. Targets, checker outcomes, group evidence and model-input certification
have distinct contracts. Preserve zeros and native nulls without imputation.

For new target-complete benchmarks, required target availability may determine
eligibility before sampling. Grouping and checker-label purity use the full
release, including target-missing rows. Target magnitudes never determine groups,
diversity or partitions. Every eligible member of a selected effective related
group stays in one partition. For frozen experiments, newer metadata, targets
or feature coverage cannot silently replace the recorded inputs.

Record the exact software revision or wheel hash and input hashes, not only a
package version. Keep target-source/endpoint definitions, eligibility decisions,
group/checker identity, assignment digest and attached outputs connected by the
workflow receipt. Model preprocessing must not silently drop or refill assigned
rows. An incomplete output directory is not a completed benchmark.

## Distribution

This repository provides results-reading and dataset APIs, not third-party
checker code or a scientific-data redistribution grant. Keep private handoffs,
retired-ID mappings, licensed CIFs and original-host logs outside public code
exports. Apply the documented source-specific permissions to each data package.
Checksums establish file integrity, not permission or scientific validity.
Exploratory splits retain `official_split=false`; a diagnostic with training
or related-group exposure is not an independent test. New training or scientific
calculations require task-specific authority, not merely use of this skill.
