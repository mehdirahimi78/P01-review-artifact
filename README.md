# P01 — Anonymous aggregate-data review supplement

**Review-only evidence package; no author-identifying metadata supplied.**

Contains three source-preserving tabular outputs from a retained empirical analysis of 19 software agents under three evidence conditions (57 retained records). Agent A10 was excluded after a prompt-assignment error; all entries in this supplement use anonymized agent IDs.

## Included tables
- `01_archived_retained_57_metrics.csv`: archived required-input recall, semantic-precondition recall, and semantic-postcondition recall; **not independently rescored**.
- `02_rq2_paired_tests_3_metrics.csv`: six archived RQ2 planned contrasts on the 14-agent documented subset; published adjusted p-values have not been independently regenerated from the raw evaluator.
- `03_threshold_sensitivity.csv`: historic 60-pair calibration and 53-pair A10-excluded threshold sensitivity, plus 20-pair holdout.

## Exclusions and limitations
- No original system prompts, documentation, traces, GT contracts, extracted YAML contracts, reviewer names, ORCID, institutional affiliation, or author identities are included.
- The R3 GT and extracted YAML evidence, including one invalid A17_S1S2.yaml source record, remain in a separate private curation package pending source licensing review.
- `Tout` (output-schema F1) is not reported as validated evidence because the historical scorer mishandled mixed schema kinds and exhibited incompatible property counts.
- Tables document archival results, not a full end-to-end reproducibility demonstration. Original execution code and evaluator have not been independently rerun here.
- Do not publish to an author-identified repository or attach a non-anonymous repository URL to a double-blind submission.

## Access and citation
Provide this file only through a submission channel approved by the conference. The current author-identified Zenodo draft is **not suitable** for double-blind reviewer access. No persistent public artifact URL or DOI is claimed by this package.

## Package checksums
See `SHA256SUMS.csv`; these hashes concern the exact included files.

## Additional holdout audit (final scientific review)

The 20 original holdout pairs (five per dimension, including the withheld output-property dimension) were joined to adjudicated human labels. At the frozen 0.70 similarity threshold, the strict-label confusion counts are TP=7, FP=5, FN=1, TN=7 (precision 0.583, recall 0.875, F1 0.700). Every false positive is classified **Partial** by human adjudication. This is a descriptive audit of the original 20-pair holdout, not a new validation set, not independent-agent generalization, and not a rescoring of the archived extraction dataset. Columns in `04_holdout_strict_audit_20.csv` include no reviewer identities, affiliations, source excerpts, or agent names. The original four dimensions contribute to the holdout, but only three are retained as primary extraction metrics in the manuscript.
