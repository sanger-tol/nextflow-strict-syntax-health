# Nextflow lint results

- Generated: 2026-05-08T00:22:00.089017401Z
- Nextflow version: 26.04.0
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/local/align_short.nf:39:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, cram ->
                          ^^^^
  ```

- Warning: `subworkflows/local/input_check.nf:25:5`: Variable was declared but not used

  ```nextflow
      reads = samplesheet_rows
      ^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
