# Nextflow lint results

- Generated: 2026-04-14T00:17:46.675347875Z
- Nextflow version: 26.03.2-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/local/genome_statistics/main.nf:204:5`: Variable was declared but not used

  ```nextflow
      multiqc = BUSCO.out.short_summaries_txt.ifEmpty([[], []])
      ^^^^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      data = samplesheet
      ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
