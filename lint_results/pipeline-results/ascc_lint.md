# Nextflow lint results

- Generated: 2026-10-08T15:33:11.535711527Z
- Nextflow version: 26.09.2-edge
- Summary: 2 errors, 10 warnings

## :x: Errors

- Error: `main.nf:159:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  workflow.onComplete {
  ^
  ```

- Error: `subworkflows/local/pe_mapping/main.nf:73:5`: Incorrect number of call arguments, expected 2 but received 4

  ```nextflow
      SAMTOOLS_MERGE(
      ^
  ```

## :warning: Warnings

- Warning: `modules/nf-core/blast/blastn/main.nf:63:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/blast/makeblastdb/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def args           = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/generate_genomes/main.nf:10:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      barcodes
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/generate_html_report/main.nf:20:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      params_file                // channel: [ params_file ]
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ascc_pipeline/main.nf:39:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_ascc_pipeline/main.nf:209:5`: Variable was declared but not used

  ```nextflow
      versions = ch_versions.mix(PREPARE_BLASTDB.out.versions)
      ^^^^^^^^
  ```

- Warning: `workflows/ascc_genomic.nf:811:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{ meta, file ->
                   ^^^^
  ```

- Warning: `workflows/ascc_genomic.nf:811:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{ meta, file ->
                         ^^^^
  ```

- Warning: `workflows/ascc_organellar.nf:588:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{ meta, file ->
                   ^^^^
  ```

- Warning: `workflows/ascc_organellar.nf:588:24`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{ meta, file ->
                         ^^^^
  ```
