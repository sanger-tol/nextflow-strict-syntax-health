# Nextflow lint results

- Generated: 2026-06-19T00:36:47.632632147Z
- Nextflow version: 26.04.3
- Summary: 11 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:109:5`: Variable was declared but not used

  ```nextflow
      ch_reference = input_fasta.map { fasta ->
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:120:5`: Variable was declared but not used

  ```nextflow
      ch_snapshot_order = params.snapshot_order ? channel.fromPath(
      ^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:138:5`: Variable was declared but not used

  ```nextflow
      ch_cram_reads   = params.cram ? fn_get_validated_channel(
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:148:5`: Variable was declared but not used

  ```nextflow
      ch_mapped_bam   = params.pre_mapped_bam ? fn_get_validated_channel(
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:158:5`: Variable was declared but not used

  ```nextflow
      ch_longreads    = fn_get_validated_channel(
      ^^^^^^^^^^^^
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

- Warning: `subworkflows/sanger-tol/repeat_masking/main.nf:31:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      repeat_intervals = WINDOWMASKER_USTAT.out.intervals
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/curationpretext.nf:314:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_collated_versions   // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
