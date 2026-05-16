# Nextflow lint results

- Generated: 2026-05-16T00:21:21.933034728Z
- Nextflow version: 26.04.1
- Summary: 10 warnings

## :warning: Warnings

- Warning: `subworkflows/local/align_long.nf:87:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .branch { meta, yaml ->
                                  ^^^^
  ```

- Warning: `subworkflows/local/align_short.nf:39:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, cram ->
                          ^^^^
  ```

- Warning: `subworkflows/local/align_short.nf:67:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam      = MERGE_OUTPUT.out.bam     // channel: [ val(meta), /path/to/bam ]
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_check.nf:25:5`: Variable was declared but not used

  ```nextflow
      reads = samplesheet_rows
      ^^^^^
  ```

- Warning: `subworkflows/local/merge_output.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bam = ch_bam                    // channel: [ val(meta), /path/to/bam ]
      ^^^^^^^^^^
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

- Warning: `workflows/readmapping.nf:162:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_collated_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
