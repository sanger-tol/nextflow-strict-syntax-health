# Nextflow lint results

- Generated: 2026-04-25T00:16:29.570726109Z
- Nextflow version: 26.03.3-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:29:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .subscribe { meta, hap1, hap2 ->
                       ^^^^
  ```
