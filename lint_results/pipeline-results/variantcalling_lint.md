# Nextflow lint results

- Generated: 2026-04-14T00:18:16.101470546Z
- Nextflow version: 26.03.2-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/variantcalling.nf:38:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_positions // channel: positions to include or exclude in the variant calling
      ^^^^^^^^^^^^
  ```
