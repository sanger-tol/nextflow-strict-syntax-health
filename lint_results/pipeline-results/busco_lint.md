# Nextflow lint results

- Generated: 2026-07-04T00:22:54.470550208Z
- Nextflow version: 26.06.0-edge
- Summary: 9 warnings

## :warning: Warnings

- Warning: `main.nf:42:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = BUSCO.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_busco_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      valid_config
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      dummy_emit = true
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:40:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, odb, ref_meta, ref -> [ ref_meta, odb, ref ] }  // meta == ref_meta thanks to APISCRIPTS_GETLINEAGEODBS
                 ^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:40:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, odb, ref_meta, ref -> [ ref_meta, odb, ref ] }  // meta == ref_meta thanks to APISCRIPTS_GETLINEAGEODBS
                     ^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:41:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .unique { meta, odb, ref ->
                               ^^^
  ```
