# Nextflow lint results

- Generated: 2026-05-01T00:19:57.434796580Z
- Nextflow version: 26.04.0
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:29:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .subscribe { meta, hap1, hap2 ->
                       ^^^^
  ```
