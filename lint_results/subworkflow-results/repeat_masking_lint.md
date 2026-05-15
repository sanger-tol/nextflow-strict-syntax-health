# Nextflow lint results

- Generated: 2026-05-15T00:23:55.102683+00:00
- Nextflow version: 26.04.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/repeat_masking/main.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      repeat_intervals = WINDOWMASKER_USTAT.out.intervals
      ^^^^^^^^^^
  ```
