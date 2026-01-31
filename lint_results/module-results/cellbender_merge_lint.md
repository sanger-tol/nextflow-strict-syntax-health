# Nextflow lint results

- Generated: 2026-01-31T00:23:25.850917+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/cellbender/merge/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      output_layer = task.ext.output_layer ?: "cellbender"
      ^^^^^^^^^^
  ```
