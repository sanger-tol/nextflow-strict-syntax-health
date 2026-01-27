# Nextflow lint results

- Generated: 2026-01-27T00:18:46.873937+00:00
- Nextflow version: 25.12.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `modules/nf-core/yara/mapper/main.nf:68:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^^^^^^^
  ```

- Warning: `modules/nf-core/yara/mapper/main.nf:70:9`: Variable was declared but not used

  ```nextflow
      def index_prefix = index[0].baseName.substring(0,index[0].baseName.lastIndexOf('.'))
          ^^^^^^^^^^
  ```
