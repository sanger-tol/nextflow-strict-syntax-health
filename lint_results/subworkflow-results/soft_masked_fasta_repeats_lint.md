# Nextflow lint results

- Generated: 2026-05-14T00:25:58.033134+00:00
- Nextflow version: 26.04.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/soft_masked_fasta_repeats/main.nf:28:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      repeats = ch_repeats // channel: [ meta, bed.gz, bed.gz.gzi, tbi?, csi? ]
      ^^^^^^^^^^
  ```
