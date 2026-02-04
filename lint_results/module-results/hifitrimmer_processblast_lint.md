# Nextflow lint results

- Generated: 2026-02-04T00:20:34.621499+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/hifitrimmer/processblast/main.nf:25:8`: Variable was declared but not used

  ```nextflow
     def prefix = task.ext.prefix ?: "${meta.id}"
         ^^^^^^^^^^
  ```
