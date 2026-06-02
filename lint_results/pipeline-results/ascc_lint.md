# Nextflow lint results

- Generated: 2026-06-02T00:32:50.179529849Z
- Nextflow version: 26.04.3
- Summary: 1 error, 35 warnings

## :x: Errors

- Error: `main.nf:159:1`: Statements cannot be mixed with script declarations -- move statements into a process, workflow, or function

  ```nextflow
  workflow.onComplete {
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

- Warning: `modules/sanger-tol/samtools/mergedup/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def args      = task.ext.args  ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/essential_jobs/main.nf:43:5`: Variable was declared but not used

  ```nextflow
      filter_fasta_sanitation_log         = FILTER_FASTA.out.sanitation_log
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/essential_jobs/main.nf:45:5`: Variable was declared but not used

  ```nextflow
      filter_fasta_length_filtering_log   = FILTER_FASTA.out.length_filtering_log
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/essential_jobs/main.nf:65:5`: Variable was declared but not used

  ```nextflow
      reference_tuple_from_GG = GENERATE_GENOME.out.reference_tuple
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/essential_jobs/main.nf:66:5`: Variable was declared but not used

  ```nextflow
      dot_genome              = GENERATE_GENOME.out.dot_genome
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/essential_jobs/main.nf:77:5`: Variable was declared but not used

  ```nextflow
      trailing_ns_report      = TRAILINGNS_CHECK.out.trailing_ns_report
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/extract_nt_blast/main.nf:79:5`: Variable was declared but not used

  ```nextflow
      ch_btk_format           = BLAST_CHUNK_TO_FULL.out.full
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/extract_nt_blast/main.nf:82:5`: Variable was declared but not used

  ```nextflow
      ch_blast_hits           = BLAST_CHUNK_TO_FULL.out.full
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/extract_nt_blast/main.nf:121:5`: Variable was declared but not used

  ```nextflow
      ch_top_lineages         = GET_LINEAGE_FOR_TOP.out.full
      ^^^^^^^^^^^^^^^
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

- Warning: `subworkflows/local/get_kmers_profile/main.nf:101:5`: Variable was declared but not used

  ```nextflow
      kmers_results = collected_files_for_combine
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/get_kmers_profile/main.nf:123:5`: Variable was declared but not used

  ```nextflow
      combined_csv    = KMER_COUNT_DIM_REDUCTION_COMBINE_CSV.out.csv
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pacbio_barcode_check/main.nf:55:5`: Variable was declared but not used

  ```nextflow
      filtered        = FILTER_BARCODE.out.debarcoded
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/run_fcsgx/main.nf:50:5`: Variable was declared but not used

  ```nextflow
      fcsgx_taxonomy_rpt  = FCSGX_RUNGX.out.taxonomy_report
      ^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_fcsgx/main.nf:74:5`: Variable was declared but not used

  ```nextflow
      fcsgxresult     = PARSE_FCSGX_RESULT.out.fcsgxresult
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_nt_kraken/main.nf:36:5`: Variable was declared but not used

  ```nextflow
      classified      = KRAKEN2_KRAKEN2.out.classified_reads_assignment
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/run_nt_kraken/main.nf:40:5`: Variable was declared but not used

  ```nextflow
      report          = KRAKEN2_KRAKEN2.out.report
      ^^^^^^
  ```

- Warning: `subworkflows/local/run_nt_kraken/main.nf:53:5`: Variable was declared but not used

  ```nextflow
      lineage         = GET_LINEAGE_FOR_KRAKEN.out.txt
      ^^^^^^^
  ```

- Warning: `subworkflows/local/run_read_coverage/main.nf:98:5`: Variable was declared but not used

  ```nextflow
      tsv_ch              = COVERM_CONTIG.out.coverage
      ^^^^^^
  ```

- Warning: `subworkflows/local/run_read_coverage/main.nf:102:5`: Variable was declared but not used

  ```nextflow
      bam_ch              = ch_out_bam
      ^^^^^^
  ```

- Warning: `subworkflows/local/run_vecscreen/main.nf:61:5`: Variable was declared but not used

  ```nextflow
      vecscreen_contam    = SUMMARISE_VECSCREEN_OUTPUT.out.vecscreen_contamination
      ^^^^^^^^^^^^^^^^
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

- Warning: `workflows/ascc.nf:141:5`: Emit name should be omitted when there is only one emit

  ```nextflow
      versions       = ch_collated_versions                 // channel: [ path(versions.yml) ]
      ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/ascc_genomic.nf:809:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter{ meta, file ->
                   ^^^^
  ```

- Warning: `workflows/ascc_genomic.nf:809:24`: Parameter was not used -- prefix with `_` to suppress warning

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
