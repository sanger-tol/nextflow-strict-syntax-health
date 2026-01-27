# Nextflow lint results

- Generated: 2026-01-27T00:18:46.843978+00:00
- Nextflow version: 25.12.0-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/scimap/mcmicro/main.nf:45:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
