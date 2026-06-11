# Nextflow lint results

- Generated: 2026-06-11T00:33:46.295049838Z
- Nextflow version: 26.04.3
- Summary: 10 warnings

## :warning: Warnings

- Warning: `main.nf:54:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      multiqc_report = GENOMENOTE.out.multiqc_report // channel: /path/to/multiqc_report.html
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:132:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def runs = meta_reads.collect { it[0].run }
                                                  ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:141:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .collect { it[1] }
                                 ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:242:5`: Variable was declared but not used

  ```nextflow
      multiqc = BUSCO.out.short_summaries_txt.ifEmpty([[], []])
      ^^^^^^^
  ```

- Warning: `subworkflows/local/get_blobtk_plots/main.nf:67:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      blobtk_images = ch_images
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:44:5`: Variable was declared but not used

  ```nextflow
      data = samplesheet
      ^^^^
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
