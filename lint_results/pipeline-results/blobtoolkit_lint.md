# Nextflow lint results

- Generated: 2026-05-18T00:22:23.102753685Z
- Nextflow version: 26.04.1
- Summary: 13 warnings

## :warning: Warnings

- Warning: `conf/modules.config:136:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename ->
                        ^^^^^^^^
  ```

- Warning: `main.nf:45:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = BLOBTOOLKIT.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/blobtools.nf:47:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      blobdir  = BLOBTOOLKIT_UPDATEBLOBDIR.out.blobdir  // channel: [ val(meta), path(dir) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:228:5`: Variable was declared but not used

  ```nextflow
      multiqc = BUSCO_BUSCO.out.short_summaries_txt
      ^^^^^^^
  ```

- Warning: `subworkflows/local/collate_stats.nf:40:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      window_tsv = BLOBTOOLKIT_WINDOWSTATS.out.tsv // channel: [ val(meta), path(window_stats_tsvs) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_alignment.nf:55:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      aln      = ch_aligned        // channel: [ val(meta), bam ]
      ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_blastx.nf:40:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      blastx_out = BLOBTOOLKIT_UNCHUNK.out.blast_out  // channel: [ val(meta), path(blastx_out) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
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

- Warning: `workflows/blobtoolkit.nf:172:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
