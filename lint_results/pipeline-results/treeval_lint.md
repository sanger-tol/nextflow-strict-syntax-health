# Nextflow lint results

- Generated: 2026-06-10T00:29:43.806827576Z
- Nextflow version: 26.04.3
- Summary: 9 warnings

## :warning: Warnings

- Warning: `modules/local/selfcomp/splitfasta/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def VERSION     = "1.7.8-1"
          ^^^^^^^
  ```

- Warning: `modules/local/selfcomp/splitfasta/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def VERSION     = "1.7.8-1"
          ^^^^^^^
  ```

- Warning: `subworkflows/local/synteny/main.nf:55:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      ch_paf              = MINIMAP2_ALIGN.out.paf
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:17:17`: Variable was declared but not used

  ```nextflow
              def kmer_len = data?.kmer_profile?.kmer_length // Will return null if not exist
                  ^^^^^^^^
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

- Warning: `workflows/treeval.nf:368:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_collated_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
