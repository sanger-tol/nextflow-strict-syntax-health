# Nextflow lint results

- Generated: 2026-05-16T00:22:09.420476+00:00
- Nextflow version: 26.04.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/soft_masked_fasta_repeats/main.nf:28:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      repeats = ch_repeats // channel: [ meta, bed.gz, bed.gz.gzi, tbi?, csi? ]
      ^^^^^^^^^^
  ```
