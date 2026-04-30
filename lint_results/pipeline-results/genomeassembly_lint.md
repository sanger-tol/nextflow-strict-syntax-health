# Nextflow lint results

- Generated: 2026-04-30T00:21:46.275235257Z
- Nextflow version: 26.04.0
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:29:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .subscribe { meta, hap1, hap2 ->
                       ^^^^
  ```
