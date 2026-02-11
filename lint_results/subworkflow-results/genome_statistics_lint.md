# Nextflow lint results

- Generated: 2026-02-11T00:14:25.269965+00:00
- Nextflow version: 26.01.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/genome_statistics/main.nf:15:5`: Variable was declared but not used

  ```nextflow
      ch_versions = channel.empty()
      ^^^^^^^^^^
  ```
