# Nextflow lint results

- Generated: 2026-02-06T13:18:21.690319058Z
- Nextflow version: 25.12.0-edge
- Summary: 13 errors, 53 warnings

## :x: Errors

- Error: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:46:9`: `base` is already declared

  ```nextflow
      def base    = "45022_3#2"
          ^^^^
  ```

- Error: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:47:9`: `chunkid` is already declared

  ```nextflow
      def chunkid = "1"
          ^^^^^^^
  ```

- Error: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:47:9`: `base` is already declared

  ```nextflow
      def base    = "45022_3#2"
          ^^^^
  ```

- Error: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:48:9`: `chunkid` is already declared

  ```nextflow
      def chunkid = "1"
          ^^^^^^^
  ```

- Error: `modules/nf-core/pretextsnapshot/main.nf:45:26`: `VERSION` is not defined

  ```nextflow
          pretextsnapshot: $VERSION
                           ^^^^^^^^
  ```

- Error: `nextflow.config:220:1`: Variable declarations cannot be mixed with config statements

  ```nextflow
  def trace_timestamp = new java.util.Date().format( 'yyyy-MM-dd_HH-mm-ss' )
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `nextflow.config:306:15`: `manifest` is not defined

  ```nextflow
  \033[0;35m  ${manifest.name} ${manifest.version}\033[0m
                ^^^^^^^^
  ```

- Error: `nextflow.config:306:32`: `manifest` is not defined

  ```nextflow
  \033[0;35m  ${manifest.name} ${manifest.version}\033[0m
                                 ^^^^^^^^
  ```

- Error: `nextflow.config:309:22`: `manifest` is not defined

  ```nextflow
      afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                       ^^^^^^^^
  ```

- Error: `nextflow.config:309:65`: `manifest` is not defined

  ```nextflow
      afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                  ^^^^^^^^
  ```

- Error: `nextflow.config:309:182`: `manifest` is not defined

  ```nextflow
      afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                                                                                       ^^^^^^^^
  ```

- Error: `nextflow.config:318:22`: `validation` is not defined

  ```nextflow
          beforeText = validation.help.beforeText
                       ^^^^^^^^^^
  ```

- Error: `nextflow.config:319:21`: `validation` is not defined

  ```nextflow
          afterText = validation.help.afterText
                      ^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^
  ```

- Warning: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/find/telomere_regions/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def find_telomere = task.ext.find_telomere ?: ''
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/local/find/telomere_regions/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def find_telomere = task.ext.find_telomere ?: ''
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/local/find/telomere_windows/main.nf:27:39`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      java ${telomere_jvm_params} -cp ${projectDir}/bin/${telomere_jar} FindTelomereWindows $file $telomere_window_cut > ${prefix}.windows
                                        ^^^^^^^^^^
  ```

- Warning: `modules/local/find/telomere_windows/main.nf:38:9`: Variable was declared but not used

  ```nextflow
      def telomere = task.ext.telomere ?: ''
          ^^^^^^^^
  ```

- Warning: `modules/local/gawk_split_directions/main.nf:26:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      suffix    = task.ext.suffix ?: "${input.collect{ it.getExtension()}.get(0)}" // use the first extension of the input files
                                                       ^^
  ```

- Warning: `modules/local/gawk_split_directions/main.nf:31:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          assert it.name != "${prefix}.${suffix}" : "Input and output names are the same, set prefix in module configuration to disambiguate!"
                 ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:26:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      suffix    = task.ext.suffix ?: "${input.collect{ it.getExtension()}.get(0)}" // use the first extension of the input files
                                                       ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:29:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz     = input.findResults{ it.getExtension().endsWith("gz") ? it.toString() : null }
                                      ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:29:72`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      lst_gz     = input.findResults{ it.getExtension().endsWith("gz") ? it.toString() : null }
                                                                         ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:31:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_cmd  = input.collect { it.toString() - ~/\.gz$/ }.join(" ")
                                   ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:34:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      cleanup    = lst_gz ? "rm ${lst_gz.collect{ it - ~/\.gz$/ }.join(" ")}" : ""
                                                  ^^
  ```

- Warning: `modules/nf-core/gawk/main.nf:37:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          assert it.name != "${prefix}.${suffix}" : "Input and output names are the same, set prefix in module configuration to disambiguate!"
                 ^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/pretextsnapshot/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def VERSION = "0.0.4"
          ^^^^^^^
  ```

- Warning: `modules/nf-core/ucsc/bedgraphtobigwig/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `nextflow.config:309:125`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      afterText = """${manifest.doi ? "\n* The pipeline\n" : ""}${manifest.doi.tokenize(",").collect { "    https://doi.org/${it.trim().replace('https://doi.org/','')}"}.join("\n")}${manifest.doi ? "\n" : ""}
                                                                                                                              ^^
  ```

- Warning: `subworkflows/local/accessory_files/main.nf:22:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/accessory_files/main.nf:23:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_empty_file       = Channel.fromPath("${baseDir}/assets/EMPTY.txt")
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/gap_finder/main.nf:14:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_maps/main.nf:23:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_maps/main.nf:83:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          hires_pretext           = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:22:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      mappedbam_ch            = Channel.empty()
      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:23:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mappedbam_ch            = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_minimap2/main.nf:24:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_minimap2/main.nf:25:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mappedbam_ch        = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/longread_coverage/main.nf:20:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      reference_index     // Channel: [ val(meta), path( reference_indx ) ]
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/longread_coverage/main.nf:25:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/longread_coverage/main.nf:110:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, my_genome_meta, my_genome ->
                                  ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/longread_coverage/main.nf:150:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_my_genome, my_genome, ref_meta, ref ->
                      ^^^^
  ```

- Warning: `subworkflows/local/longread_coverage/main.nf:150:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_my_genome, my_genome, ref_meta, ref ->
                                  ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/longread_coverage/main.nf:150:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_my_genome, my_genome, ref_meta, ref ->
                                                                       ^^^
  ```

- Warning: `subworkflows/local/repeat_density/main.nf:27:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/repeat_density/main.nf:159:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          GNU_SORT_B.out.sorted.map { it[1] }
                                      ^^
  ```

- Warning: `subworkflows/local/telo_extraction/main.nf:9:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/telo_extraction/main.nf:21:50`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def safe_windows    = windows_file.ifEmpty { Channel.empty() }
                                                   ^^^^^^^
  ```

- Warning: `subworkflows/local/telo_finder/main.nf:18:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:82:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      input_fasta     = Channel.fromPath(
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:88:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      cram_dir        = Channel.fromPath(
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:120:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_reads        = Channel
                        ^^^^^^^
  ```

- Warning: `workflows/curationpretext.nf:35:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/curationpretext.nf:36:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_empty_file       = Channel.fromPath("${baseDir}/assets/EMPTY.txt")
                            ^^^^^^^
  ```

- Warning: `workflows/curationpretext.nf:40:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, file ->
                    ^^^^
  ```

- Warning: `workflows/curationpretext.nf:58:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      unzipped_input = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `workflows/curationpretext.nf:186:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/curationpretext.nf:210:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/curationpretext.nf:212:5`: Variable was declared but not used

  ```nextflow
      summary_params      = paramsSummaryMap(
      ^^^^^^^^^^^^^^
  ```
