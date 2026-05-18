# Nextflow lint results

- Generated: 2026-05-18T00:22:45.213319+00:00
- Nextflow version: 26.04.1
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/repeat_masking/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      repeat_intervals = WINDOWMASKER_USTAT.out.intervals
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/repeat_masking/main.nf:34:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      repeat_intervals
      ^^^^^^^^^^
  ```
