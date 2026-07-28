# Nextflow lint results

- Generated: 2026-07-28T00:21:25.213694+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/autofilter/filterfasta/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def args2       = task.ext.args2    ?: ''
          ^^^^^^^^^^
  ```
