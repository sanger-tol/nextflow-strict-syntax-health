# Nextflow lint results

- Generated: 2026-05-20T00:27:57.566151+00:00
- Nextflow version: 26.04.1
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/soft_masked_fasta_repeats/main.nf:28:5`: Variable was declared but not used

  ```nextflow
      repeats = ch_repeats
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/soft_masked_fasta_repeats/main.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      repeats // channel: [ meta, bed.gz, bed.gz.gzi, tbi?, csi? ]
      ^^^^^^^^^^
  ```
