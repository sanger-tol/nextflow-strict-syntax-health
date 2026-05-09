# Nextflow lint results

- Generated: 2026-05-09T00:20:51.693112200Z
- Nextflow version: 26.04.0
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/local/genome_statistics/main.nf:131:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  def runs = meta_reads.collect { it[0].run }
                                                  ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:140:32`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                      .collect { it[1] }
                                 ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:237:5`: Variable was declared but not used

  ```nextflow
      multiqc = BUSCO.out.short_summaries_txt.ifEmpty([[], []])
      ^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:44:5`: Variable was declared but not used

  ```nextflow
      data = samplesheet
      ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
