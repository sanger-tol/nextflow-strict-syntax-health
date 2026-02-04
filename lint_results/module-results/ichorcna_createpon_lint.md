# Nextflow lint results

- Generated: 2026-02-04T00:20:34.625620+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/ichorcna/createpon/main.nf:31:9`: `exons` is already declared

  ```nextflow
      def exons  = exons           ? "exons.bed='${exons}',"                : ''
          ^^^^^^^^^^
  ```
