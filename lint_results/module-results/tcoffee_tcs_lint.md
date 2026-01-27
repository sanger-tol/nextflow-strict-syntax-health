# Nextflow lint results

- Generated: 2026-01-27T00:18:46.862381+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/tcoffee/tcs/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args          = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/tcoffee/tcs/main.nf:63:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```
