# Nextflow lint results

- Generated: 2026-06-06T00:26:06.348181111Z
- Nextflow version: 26.04.3
- Summary: 10 warnings

## :warning: Warnings

- Warning: `subworkflows/local/filter_pacbio.nf:65:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      fastq    = SAMTOOLS_FASTQ.out.other // channel: [ meta, /path/to/fastq ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_filter_split.nf:19:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_split = fasta.map { meta, fa, fai -> [meta, fa] }
                                                 ^^^
  ```

- Warning: `subworkflows/local/input_filter_split.nf:48:5`: Emit name should be omitted when there is only one emit

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

- Warning: `workflows/variantcalling.nf:55:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      }.branch { meta, fa ->
                 ^^^^
  ```

- Warning: `workflows/variantcalling.nf:186:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions = ch_collated_versions // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```
