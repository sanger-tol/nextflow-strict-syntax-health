# Nextflow lint results

- Generated: 2026-04-16T23:45:51.754613995Z
- Nextflow version: 26.03.2-edge
- Summary: 6 warnings

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

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
