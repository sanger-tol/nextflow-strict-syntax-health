# Nextflow lint results

- Generated: 2026-05-16T00:21:38.041573941Z
- Nextflow version: 26.04.1
- Summary: 7 warnings

## :warning: Warnings

- Warning: `subworkflows/local/fasta_windows.nf:73:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      bedgraph = ch_bedgraph
      ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/params_check.nf:59:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      fasta_fai = ch_fasta_fai // channel: [ val(meta), path/to/fasta, path/to/fai ]
      ^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/sequencecomposition.nf:85:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_collated_versions // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
