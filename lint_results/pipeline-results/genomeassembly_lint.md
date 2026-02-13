# Nextflow lint results

- Generated: 2026-02-13T00:09:42.205878468Z
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/polishing/main.nf:66:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { spec, fasta, bed_chunks, lr_bam, lr_bai, lr_csv, vcf, tbi ->
                                  ^^^^^^^^^^
  ```
