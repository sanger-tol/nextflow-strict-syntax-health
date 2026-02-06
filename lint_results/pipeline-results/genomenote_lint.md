# Nextflow lint results

- Generated: 2026-02-06T15:23:55.310418987Z
- Nextflow version: 25.12.0-edge
- Summary: 27 errors, 82 warnings

## :x: Errors

- Error: `conf/base.config:43:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(4, 2*task.attempt, 1, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:55:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(4, 2*task.attempt, 1, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:71:68`: `positive_log` is not defined

  ```nextflow
          memory = { 1.GB * Math.pow(2, 3 + task.attempt + Math.ceil(positive_log(meta.genome_size/1000000000, 2)))  }
                                                                     ^^^^^^^^^^^^
  ```

- Error: `conf/base.config:72:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(4, 4*task.attempt, Math.ceil(meta.genome_size/1000000000), 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:77:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(2, 2*task.attempt, 1, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:90:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(2, 2*task.attempt, 1, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:109:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(2, 2*task.attempt, 1, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/local/combine_metadata.nf:24:5`: `for` loops are no longer supported

  ```nextflow
      for (item in  file_list){
      ^^^
  ```

- Error: `modules/local/combine_metadata.nf:24:10`: `item` is not defined

  ```nextflow
      for (item in  file_list){
           ^^^^
  ```

- Error: `modules/local/combine_metadata.nf:25:20`: `item` is not defined

  ```nextflow
          def file = item
                     ^^^^
  ```

- Error: `modules/local/combine_metadata.nf:26:24`: `item` is not defined

  ```nextflow
          def file_ext = item.getExtension()
                         ^^^^
  ```

- Error: `modules/local/combine_metadata.nf:27:32`: `item` is not defined

  ```nextflow
          def file_name = "--" + item.getName().minus("${prefix}_").minus(".${file_ext}").toLowerCase() + "_file"
                                 ^^^^
  ```

- Error: `modules/local/upload_higlass_data.nf:14:9`: `map_uuid` is not defined

  ```nextflow
      env map_uuid, emit: map_uuid
          ^^^^^^^^
  ```

- Error: `modules/local/upload_higlass_data.nf:15:9`: `grid_uuid` is not defined

  ```nextflow
      env grid_uuid, emit: grid_uuid
          ^^^^^^^^^
  ```

- Error: `modules/local/upload_higlass_data.nf:16:9`: `file_name` is not defined

  ```nextflow
      env file_name, emit: file_name
          ^^^^^^^^^
  ```

- Error: `modules/local/write_to_database.nf:5:5`: Invalid process directive

  ```nextflow
      tag = ""
      ^^^^^^^^
  ```

- Error: `modules/nf-core/blobtk/plot/main.nf:9:5`: Invalid process directive

  ```nextflow
      errorStrategy = 'ignore'
      ^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/blobtk/plot/main.nf:55:9`: `prefix` is already declared

  ```nextflow
      def prefix  = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Error: `modules/nf-core/genescopefk/main.nf:18:26`: `KMERCOV` is not defined

  ```nextflow
      tuple val(meta), env(KMERCOV)                         , emit: kmer_cov
                           ^^^^^^^
  ```

- Error: `nextflow.config:354:17`: Unexpected input: '('

  ```nextflow
  def positive_log(value, base) {
                  ^
  ```

- Error: `subworkflows/local/genome_statistics/main.nf:168:52`: `haplotype` is already declared

  ```nextflow
      | map { meta, hist, ktab, meta2, fasta, meta3, haplotype ->
                                                     ^^^^^^^^^
  ```

- Error: `subworkflows/local/get_blobtk_plots/main.nf:47:28`: `fasta` is already declared

  ```nextflow
          | multiMap { meta, fasta, local, online, btk_args ->
                             ^^^^^
  ```

- Error: `subworkflows/local/input_check/main.nf:20:9`: Variables in a closure should be declared with `def`

  ```nextflow
          meta = [
          ^^^^
  ```

- Error: `subworkflows/local/input_check/main.nf:42:16`: `meta` is already declared

  ```nextflow
          .map { meta ->
                 ^^^^
  ```

- Error: `subworkflows/local/input_check/main.nf:49:16`: `meta` is already declared

  ```nextflow
          .map { meta, datafile -> [meta.assembly, meta, datafile] }
                 ^^^^
  ```

- Error: `subworkflows/local/input_check/main.nf:51:26`: `meta` is already declared

  ```nextflow
          .map { assembly, meta, datafile, meta2 ->
                           ^^^^
  ```

- Error: `workflows/genomenote.nf:136:9`: Variables in a closure should be declared with `def`

  ```nextflow
          flagstat = file( reads.resolveSibling( reads.baseName + ".flagstat" ), checkIfExists: true)
          ^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/createtable.nf:30:43`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def hic = meta3s.collect { "--hic " + it.id } .join(' ')
                                            ^^
  ```

- Warning: `modules/local/createtable.nf:31:95`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fst = (flagstats instanceof List ? flagstats : [flagstats]).collect { "--flagstat " + it } .join(' ')
                                                                                                ^^
  ```

- Warning: `modules/local/filter/bed.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ncbidatasets/get_chromlist.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/ncbidatasets/get_odb.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/restructurebuscodir.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/restructurebuscodir.nf:22:5`: Variable was declared but not used

  ```nextflow
      prefix = task.ext.prefix ?: "${meta.id}"
      ^^^^^^
  ```

- Warning: `modules/nf-core/cooler/dump/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:26:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:30:61`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def args_sorted = args.replaceAll(/(.*)(-[wxy])(.*)/) { all, pre, param, post -> "$pre $post $param" }.trim()
                                                              ^^^
  ```

- Warning: `modules/nf-core/gffread/main.nf:49:103`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def extension   = args.contains("-T")       ? 'gtf' : ( ( ['-w', '-x', '-y' ].any { args.contains(it) } ) ? 'fasta' : 'gff3' )
                                                                                                        ^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:47:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      fk_ktab     = fastk_ktab ? "${fastk_ktab.find{ it.toString().endsWith(".ktab") }}" : ''
                                                     ^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:48:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      mat_hapktab = mathaptab  ? "${mathaptab.find{ it.toString().endsWith(".ktab") }}"  : ''
                                                    ^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:49:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      pat_hapktab = pathaptab  ? "${pathaptab.find{ it.toString().endsWith(".ktab") }}"  : ''
                                                    ^^
  ```

- Warning: `modules/sanger-tol/ancestral/extract/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ''
          ^^^^
  ```

- Warning: `modules/sanger-tol/ancestral/extract/main.nf:27:9`: Variable was declared but not used

  ```nextflow
      def prefix  = task.ext.prefix   ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/sanger-tol/ancestral/plot/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ''
          ^^^^
  ```

- Warning: `modules/sanger-tol/ancestral/plot/main.nf:44:9`: Variable was declared but not used

  ```nextflow
      def prefix  = task.ext.prefix   ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `subworkflows/local/annotation_ancestral/main.nf:23:39`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions                     = Channel.empty()
                                        ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation_statistics/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/annotation_statistics/main.nf:57:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, fasta -> fasta }
              ^^^^
  ```

- Warning: `subworkflows/local/combine_note_data/main.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/combine_note_data/main.nf:59:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_api_url = Channel.of(params.genome_notes_api)
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/contact_maps/main.nf:21:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/contact_maps/main.nf:55:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          cooler_file = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/contact_maps/main.nf:56:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          mcool_file  = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/contact_maps/main.nf:57:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          grid_file   = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/contact_maps/main.nf:58:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          link_file   = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/contact_maps/main.nf:75:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          pretext_map = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/contact_maps/main.nf:76:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          pretext_png = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_metadata/main.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_metadata/main.nf:75:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gbif_params = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_metadata/main.nf:78:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, it ->
                    ^^
  ```

- Warning: `subworkflows/local/genome_metadata/main.nf:96:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, it ->
                    ^^
  ```

- Warning: `subworkflows/local/genome_metadata/main.nf:120:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, it ->
                    ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:28:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:62:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_lineage      = Channel.of(params.busco_lineage)
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:75:17`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          | map { meta, csv -> csv }
                  ^^^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:116:9`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, file ->
          ^^^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:159:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dir.listFiles().findAll { it.toString().endsWith(".hist") } .collect(),
                                    ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:160:35`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dir.listFiles().findAll { it.toString().contains(".ktab") } .collect(),
                                    ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:168:45`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, hist, ktab, meta2, fasta, meta3, haplotype ->
                                              ^^^^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:208:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              lmf.collect { it[0] },
                            ^^
  ```

- Warning: `subworkflows/local/genome_statistics/main.nf:209:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              lmf.collect { it[1] },
                            ^^
  ```

- Warning: `subworkflows/local/get_blobtk_plots/main.nf:12:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/get_blobtk_plots/main.nf:20:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      blobtk_arguments = Channel.of(
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/get_blobtk_plots/main.nf:44:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          | combine(btk_local_path.map{ [it] })
                                         ^^
  ```

- Warning: `subworkflows/local/get_blobtk_plots/main.nf:45:41`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          | combine(btk_online_path.map{ [it] })
                                          ^^
  ```

- Warning: `subworkflows/local/higlass_generation/main.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/higlass_generation/main.nf:19:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_higlass_link = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/higlass_generation/main.nf:49:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, list -> list }
              ^^^^
  ```

- Warning: `subworkflows/local/higlass_generation/main.nf:59:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, cool, bin -> [ meta, cool ] }
                          ^^^
  ```

- Warning: `subworkflows/local/higlass_generation/main.nf:68:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, cool, bin -> [ meta, cool, [] ] }
                          ^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:29:13`: Mutating an external variable in an operator closure can lead to a race condition

  ```nextflow
              meta.biosample_hic = row.hic_biosample
              ^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:33:13`: Mutating an external variable in an operator closure can lead to a race condition

  ```nextflow
              meta.biosample_rna = row.rna_biosample
              ^^^^
  ```

- Warning: `subworkflows/local/input_check/main.nf:51:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { assembly, meta, datafile, meta2 ->
                 ^^^^^^^^
  ```

- Warning: `subworkflows/local/pretext_generation/main.nf:8:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      chrom_list      // Channel [ val(meta), path(file)      ]
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pretext_generation/main.nf:12:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:115:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_metadata = Channel.of(metadata_inputs)
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:124:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_lineage_db = Channel.fromPath(params.lineage_db).first()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:126:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_lineage_db = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:129:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_cool_order = Channel.fromPath(params.cool_order).first()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:131:25`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_cool_order = Channel.empty()
                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:134:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_ancestral_table = Channel.fromPath(params.ancestral_table).map { path -> [[id: path.getBaseName()], path] }
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:136:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_ancestral_table = Channel.empty()
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:139:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_btk_local_path = Channel.fromPath(params.btk_location, type: "dir")
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:141:29`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_btk_local_path = Channel.of([])
                              ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:144:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_btk_online_path = Channel.of(params.btk_online_location)
                               ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genomenote_pipeline/main.nf:146:30`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_btk_online_path = Channel.of([])
                               ^^^^^^^
  ```

- Warning: `workflows/genomenote.nf:81:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, haplotype -> haplotype }
                 ^^^^
  ```

- Warning: `workflows/genomenote.nf:94:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | branch { meta, fasta ->
                 ^^^^
  ```

- Warning: `workflows/genomenote.nf:135:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map{ meta, reads, blank ->
                          ^^^^^
  ```

- Warning: `workflows/genomenote.nf:172:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.of(params.binsize),
          ^^^^^^^
  ```

- Warning: `workflows/genomenote.nf:182:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_annotation_stats = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/genomenote.nf:185:13`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              Channel.fromPath(params.annotation_set),
              ^^^^^^^
  ```

- Warning: `workflows/genomenote.nf:199:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_file_list = Channel.fromPath("$projectDir/assets/genome_metadata_template.csv")
                         ^^^^^^^
  ```

- Warning: `workflows/genomenote.nf:239:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/genomenote.nf:295:65`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(ch_flagstat.collect{it[1]}.ifEmpty([]))
                                                                  ^^
  ```

- Warning: `workflows/genomenote.nf:296:83`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_multiqc_files = ch_multiqc_files.mix(GENOME_STATISTICS.out.multiqc.collect{it[1]}.ifEmpty([]))
                                                                                    ^^
  ```
