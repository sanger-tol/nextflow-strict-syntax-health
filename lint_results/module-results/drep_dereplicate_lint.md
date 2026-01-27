# Nextflow lint results

- Generated: 2026-01-27T00:18:46.753292+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/drep/dereplicate/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^^^^^
  ```
