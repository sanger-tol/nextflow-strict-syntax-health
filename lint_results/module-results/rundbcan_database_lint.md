# Nextflow lint results

- Generated: 2026-02-04T00:20:34.688898+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/rundbcan/database/main.nf:17:9`: Variable was declared but not used

  ```nextflow
      def args   = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/rundbcan/database/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
