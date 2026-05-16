# Nextflow lint results

- Generated: 2026-05-16T00:21:51.287511728Z
- Nextflow version: 26.04.1
- Summary: 8 warnings

## :warning: Warnings

- Warning: `subworkflows/local/filter_pacbio.nf:65:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      fastq    = SAMTOOLS_FASTQ.out.other // channel: [ meta, /path/to/fastq ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_filter_split.nf:64:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      reads_fasta = cram_crai_fasta_fai // channel: [ val(meta), cram, crai, intervals, val(meta_fasta), fasta, [], fai ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_merge.nf:58:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      merged_reads = merged_reads
      ^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/variantcalling.nf:162:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_collated_versions // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
