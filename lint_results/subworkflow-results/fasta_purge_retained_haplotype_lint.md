# Nextflow lint results

- Generated: 2026-04-24T00:20:12.020449+00:00
- Nextflow version: 26.03.3-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:29:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .subscribe { meta, hap1, hap2 ->
                       ^^^^^^^^^^
  ```
