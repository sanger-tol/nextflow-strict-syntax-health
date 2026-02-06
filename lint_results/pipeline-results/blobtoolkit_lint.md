# Nextflow lint results

- Generated: 2026-02-06T15:22:42.917342565Z
- Nextflow version: 25.12.0-edge
- Summary: 60 errors, 94 warnings

## :x: Errors

- Error: `conf/base.config:57:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(4, 2*task.attempt, meta.read_count/1000000, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:58:29`: `log_increase_cpus` is not defined

  ```nextflow
          memory = { 800.MB * log_increase_cpus(4, 2*task.attempt, meta.read_count/1000000, 2) + 14.GB * Math.ceil( Math.pow(meta2.genome_size / 1000000000, 0.6)) * task.attempt }
                              ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:64:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(4, 2*task.attempt, meta.read_count/1000000, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:65:29`: `log_increase_cpus` is not defined

  ```nextflow
          memory = { 800.MB * log_increase_cpus(4, 2*task.attempt, meta.read_count/1000000, 2) + 30.GB * Math.ceil( Math.pow(meta2.genome_size / 1000000000, 0.6)) * task.attempt }
                              ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:71:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(4, 2*task.attempt, meta.read_count/1000000, 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:72:29`: `log_increase_cpus` is not defined

  ```nextflow
          memory = { 800.MB * log_increase_cpus(4, 2*task.attempt, meta.read_count/1000000, 2) + 14.GB * Math.ceil( Math.pow(meta2.genome_size / 1000000000, 0.6)) * task.attempt }
                              ^^^^^^^^^^^^^^^^^
  ```

- Error: `conf/base.config:103:68`: `positive_log` is not defined

  ```nextflow
          memory = { 1.GB * Math.pow(2, 3 + task.attempt + Math.ceil(positive_log(meta.genome_size/1000000000, 2))) }
                                                                     ^^^^^^^^^^^^
  ```

- Error: `conf/base.config:104:20`: `log_increase_cpus` is not defined

  ```nextflow
          cpus   = { log_increase_cpus(4, 4*task.attempt, Math.ceil(meta.genome_size/1000000000), 2) }
                     ^^^^^^^^^^^^^^^^^
  ```

- Error: `modules/local/blobtk/depth.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtk/images.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/chunk.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/countbuscos.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/countbuscos.nf:12:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(bed)
                ^^^^
  ```

- Error: `modules/local/blobtoolkit/createblobdir.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/extractbuscos.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/summary.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/unchunk.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/updateblobdir.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/updatemeta.nf:5:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/blobtoolkit/windowstats.nf:4:5`: Invalid process directive

  ```nextflow
      if (workflow.profile.tokenize(',').intersect(['conda', 'mamba']).size() >= 1) {
      ^
  ```

- Error: `modules/local/nohit_list.nf:12:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(fasta)      //path to genome fasta file
                ^^^^
  ```

- Error: `modules/local/windowstats_input.nf:11:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(mononuc)
                ^^^^
  ```

- Error: `modules/local/windowstats_input.nf:12:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(depth)
                ^^^^
  ```

- Error: `modules/local/windowstats_input.nf:13:15`: `meta` is already declared

  ```nextflow
      tuple val(meta), path(countbusco)
                ^^^^
  ```

- Error: `modules/nf-core/diamond/blastp/main.nf:38:30`: Unexpected input: '='

  ```nextflow
          case "blast": outfmt = 0; break
                               ^
  ```

- Error: `modules/nf-core/diamond/blastx/main.nf:39:30`: Unexpected input: '='

  ```nextflow
          case "blast": outfmt = 0; break
                               ^
  ```

- Error: `nextflow.config:387:17`: Unexpected input: '('

  ```nextflow
  def positive_log(value, base) {
                  ^
  ```

- Error: `subworkflows/local/busco_diamond_blastp.nf:7:1`: Module could not be parsed: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/pipelines/blobtoolkit/modules/nf-core/diamond/blastp/main.nf'

  ```nextflow
  include { DIAMOND_BLASTP            } from '../../modules/nf-core/diamond/blastp/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/busco_diamond_blastp.nf:60:19`: `fasta` is already declared

  ```nextflow
              meta, fasta -> [meta.lineage_name, [meta, fasta]]
                    ^^^^^
  ```

- Error: `subworkflows/local/busco_diamond_blastp.nf:64:24`: `fasta` is already declared

  ```nextflow
              def (meta, fasta) = fasta_data
                         ^^^^^
  ```

- Error: `subworkflows/local/busco_diamond_blastp.nf:80:22`: `fasta` is already declared

  ```nextflow
          .map { meta, fasta ->
                       ^^^^^
  ```

- Error: `subworkflows/local/busco_diamond_blastp.nf:203:5`: `DIAMOND_BLASTP` is not defined

  ```nextflow
      DIAMOND_BLASTP (
      ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/busco_diamond_blastp.nf:210:37`: `DIAMOND_BLASTP` is not defined

  ```nextflow
      ch_versions = ch_versions.mix ( DIAMOND_BLASTP.out.versions.first() )
                                      ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/busco_diamond_blastp.nf:250:19`: `DIAMOND_BLASTP` is not defined

  ```nextflow
      blastp_txt  = DIAMOND_BLASTP.out.txt  // channel: [ val(meta), path(txt) ]
                    ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/coverage_stats.nf:81:31`: `fasta` is already declared

  ```nextflow
      | map { meta, bed, meta2, fasta -> [ meta2, bed ] }
                                ^^^^^
  ```

- Error: `subworkflows/local/input_check.nf:302:25`: Unexpected input: '\n'

  ```nextflow
          case "ILLUMINA":
                          ^
  ```

- Error: `subworkflows/local/run_blastn.nf:81:28`: `fasta` is already declared

  ```nextflow
          | map { meta, txt, fasta -> [meta, fasta] }
                             ^^^^^
  ```

- Error: `subworkflows/local/run_blastx.nf:7:1`: Module could not be parsed: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/pipelines/blobtoolkit/modules/nf-core/diamond/blastx/main.nf'

  ```nextflow
  include { DIAMOND_BLASTX      } from '../../modules/nf-core/diamond/blastx/main'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_blastx.nf:34:5`: `DIAMOND_BLASTX` is not defined

  ```nextflow
      DIAMOND_BLASTX ( BLOBTOOLKIT_CHUNK.out.chunks, blastx, outext, cols, taxon_id )
      ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_blastx.nf:35:37`: `DIAMOND_BLASTX` is not defined

  ```nextflow
      ch_versions = ch_versions.mix ( DIAMOND_BLASTX.out.versions.first() )
                                      ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/run_blastx.nf:41:27`: `DIAMOND_BLASTX` is not defined

  ```nextflow
      BLOBTOOLKIT_UNCHUNK ( DIAMOND_BLASTX.out.txt )
                            ^^^^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:12:1`: Module could not be parsed: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/pipelines/blobtoolkit/subworkflows/local/input_check.nf'

  ```nextflow
  include { INPUT_CHECK        } from '../subworkflows/local/input_check'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:64:5`: `INPUT_CHECK` is not defined

  ```nextflow
      INPUT_CHECK (
      ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:72:45`: `INPUT_CHECK` is not defined

  ```nextflow
      ch_versions         = ch_versions.mix ( INPUT_CHECK.out.versions )
                                              ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:79:30`: `INPUT_CHECK` is not defined

  ```nextflow
          MINIMAP2_ALIGNMENT ( INPUT_CHECK.out.reads, ch_prepared_genome )
                               ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:83:27`: `INPUT_CHECK` is not defined

  ```nextflow
          ch_aligned      = INPUT_CHECK.out.reads
                            ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:99:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.busco_lineages,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:100:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.busco_db,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:101:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.odb_version,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:102:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.blastp,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:103:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.taxon_id,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:104:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.precomputed_busco,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:116:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.blastx,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:117:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.taxon_id,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:129:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.blastn,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:130:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.taxon_id,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:152:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.config,
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:153:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.synonyms_tsv.ifEmpty([[],[]]),
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:154:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.categories_tsv.ifEmpty([[],[]]),
          ^^^^^^^^^^^
  ```

- Error: `workflows/blobtoolkit.nf:160:9`: `INPUT_CHECK` is not defined

  ```nextflow
          INPUT_CHECK.out.taxdump
          ^^^^^^^^^^^
  ```

## :warning: Warnings

- Warning: `modules/local/blobtoolkit/countbuscos.nf:11:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(table, stageAs: 'dir??/*')
                ^^^^
  ```

- Warning: `modules/local/blobtoolkit/countbuscos.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/blobtoolkit/countbuscos.nf:24:80`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def busco_inputs = (table instanceof List ? table : [table]).collect{"--in $it"}.join(' ')
                                                                                 ^^
  ```

- Warning: `modules/local/blobtoolkit/createblobdir.nf:27:87`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def busco_args = (busco instanceof List ? busco : [busco]).collect { "--busco " + it } .join(' ')
                                                                                        ^^
  ```

- Warning: `modules/local/blobtoolkit/extractbuscos.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/blobtoolkit/extractbuscos.nf:24:79`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def seq_args = (seq instanceof List ? seq : [seq]).collect { "--busco " + it } .join(' ')
                                                                                ^^
  ```

- Warning: `modules/local/compressblobdir.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/generate_config.nf:29:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/generate_config.nf:33:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_reads = reads.collect{"--read_id ${it[0].id} --read_type ${it[0].datatype} --read_layout ${it[0].layout} --read_path ${it[1]}"}.join(' ')
                                                   ^^
  ```

- Warning: `modules/local/generate_config.nf:33:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_reads = reads.collect{"--read_id ${it[0].id} --read_type ${it[0].datatype} --read_layout ${it[0].layout} --read_path ${it[1]}"}.join(' ')
                                                                           ^^
  ```

- Warning: `modules/local/generate_config.nf:33:106`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_reads = reads.collect{"--read_id ${it[0].id} --read_type ${it[0].datatype} --read_layout ${it[0].layout} --read_path ${it[1]}"}.join(' ')
                                                                                                           ^^
  ```

- Warning: `modules/local/generate_config.nf:33:134`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_reads = reads.collect{"--read_id ${it[0].id} --read_type ${it[0].datatype} --read_layout ${it[0].layout} --read_path ${it[1]}"}.join(' ')
                                                                                                                                       ^^
  ```

- Warning: `modules/local/generate_config.nf:34:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_databases = db_paths.collect{"--${it[0].type} ${it[1]}"}.join(' ')
                                                  ^^
  ```

- Warning: `modules/local/generate_config.nf:34:63`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_databases = db_paths.collect{"--${it[0].type} ${it[1]}"}.join(' ')
                                                                ^^
  ```

- Warning: `modules/local/nohit_list.nf:11:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(blast)      //path to blast output table in txt format
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

- Warning: `modules/local/windowstats_input.nf:10:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(freq)
                ^^^^
  ```

- Warning: `modules/local/windowstats_input.nf:11:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(mononuc)
                ^^^^
  ```

- Warning: `modules/local/windowstats_input.nf:12:15`: Variable was declared but not used

  ```nextflow
      tuple val(meta), path(depth)
                ^^^^
  ```

- Warning: `modules/nf-core/blast/blastn/main.nf:83:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:23:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list = files_in.collect { it.toString() }
                                         ^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:58:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list   = files_in.collect { it.toString() }
                                           ^^
  ```

- Warning: `modules/nf-core/fastawindows/main.nf:41:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:66:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/pigz/compress/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/blobtools.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:22:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:32:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.from(basal_lineages)
      ^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:63:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { lineage, fasta_data, busco_data ->
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:65:18`: Variable was declared but not used

  ```nextflow
              def (busco_meta, busco_dir) = busco_data ?: [null, null]
                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:71:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          precomputed: it[0].busco_dir != null
                       ^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:80:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, fasta ->
                       ^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:82:17`: Variable was declared but not used

  ```nextflow
              def lineage = meta.lineage_name
                  ^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:105:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ch_busco_to_run.to_compute.map { it[0].lineage_name },
                                           ^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:173:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | collect(flat: false) { lineage_name, meta, outputs -> outputs.seq_dir }
                               ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:173:44`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | collect(flat: false) { lineage_name, meta, outputs -> outputs.seq_dir }
                                             ^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:191:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[1].size() > 140 &&
                    ^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:218:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          | filter { meta, outputs -> outputs.full_table }
                     ^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:221:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def cleaned_meta = meta.findAll { it.key != "lineage_name" && it.key != "lineage_index" && it.key != "busco_dir" }
                                                ^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:221:75`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def cleaned_meta = meta.findAll { it.key != "lineage_name" && it.key != "lineage_index" && it.key != "busco_dir" }
                                                                            ^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:221:104`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              def cleaned_meta = meta.findAll { it.key != "lineage_name" && it.key != "lineage_index" && it.key != "busco_dir" }
                                                                                                         ^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:232:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  table_positions.sort { a, b -> a[1] <=> b[1] }.collect { it[0] }
                                                                           ^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:244:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, outputs -> outputs }
                 ^^^^
  ```

- Warning: `subworkflows/local/collate_stats.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/coverage_stats.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/coverage_stats.nf:81:13`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, bed, meta2, fasta -> [ meta2, bed ] }
              ^^^^
  ```

- Warning: `subworkflows/local/coverage_stats.nf:81:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      | map { meta, bed, meta2, fasta -> [ meta2, bed ] }
                                ^^^^^
  ```

- Warning: `subworkflows/local/finalise_blobdir.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_alignment.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/minimap_alignment.nf:25:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          meta, reads ->
                ^^^^^
  ```

- Warning: `subworkflows/local/minimap_alignment.nf:53:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:16:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/prepare_genome.nf:22:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, fasta ->
                    ^^^^
  ```

- Warning: `subworkflows/local/run_blastn.nf:23:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/run_blastn.nf:37:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          NOHIT_LIST.out.nohitlist.map { meta, nohit -> nohit } . filter { it.size() > 0 }
                                         ^^^^
  ```

- Warning: `subworkflows/local/run_blastn.nf:37:74`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          NOHIT_LIST.out.nohitlist.map { meta, nohit -> nohit } . filter { it.size() > 0 }
                                                                           ^^
  ```

- Warning: `subworkflows/local/run_blastn.nf:50:16`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      | filter { it[1].size() > 0 }
                 ^^
  ```

- Warning: `subworkflows/local/run_blastn.nf:61:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
              not_empty: Channel.empty()
                         ^^^^^^^
  ```

- Warning: `subworkflows/local/run_blastn.nf:72:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          | branch { meta, txt ->
                     ^^^^
  ```

- Warning: `subworkflows/local/run_blastn.nf:81:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          | map { meta, txt, fasta -> [meta, fasta] }
                        ^^^
  ```

- Warning: `subworkflows/local/run_blastx.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:107:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_fasta = Channel.value([ [ 'id': params.accession ?: file(params.fasta.replace(".gz", "")).baseName ], file(params.fasta) ])
                 ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:109:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.empty()
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:110:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( Channel.fromPath(params.blastn).map { tuple(["type": "blastn"], it) } )
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:110:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( Channel.fromPath(params.blastn).map { tuple(["type": "blastn"], it) } )
                                                                                   ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:111:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( Channel.fromPath(params.blastx).map { tuple(["type": "blastx"], it) } )
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:111:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( Channel.fromPath(params.blastx).map { tuple(["type": "blastx"], it) } )
                                                                                   ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:112:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( Channel.fromPath(params.blastp).map { tuple(["type": "blastp"], it) } )
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:112:82`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( Channel.fromPath(params.blastp).map { tuple(["type": "blastp"], it) } )
                                                                                   ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:113:45`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( params.precomputed_busco ? Channel.fromPath(params.precomputed_busco).map { tuple([ "type": "precomputed_busco"], it ) } : Channel.empty() )
                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:113:132`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( params.precomputed_busco ? Channel.fromPath(params.precomputed_busco).map { tuple([ "type": "precomputed_busco"], it ) } : Channel.empty() )
                                                                                                                                     ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:113:141`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( params.precomputed_busco ? Channel.fromPath(params.precomputed_busco).map { tuple([ "type": "precomputed_busco"], it ) } : Channel.empty() )
                                                                                                                                              ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:114:33`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( params.busco ? Channel.fromPath(params.busco).map { tuple([ "type": "busco"], it ) } : Channel.empty() )
                                  ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:114:96`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( params.busco ? Channel.fromPath(params.busco).map { tuple([ "type": "busco"], it ) } : Channel.empty() )
                                                                                                 ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:114:105`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( params.busco ? Channel.fromPath(params.busco).map { tuple([ "type": "busco"], it ) } : Channel.empty() )
                                                                                                          ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:115:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          .concat( Channel.fromPath(params.taxdump).map { tuple(["type": "taxdump"], it) } )
                   ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_blobtoolkit_pipeline/main.nf:115:84`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .concat( Channel.fromPath(params.taxdump).map { tuple(["type": "taxdump"], it) } )
                                                                                     ^^
  ```

- Warning: `subworkflows/local/view.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:46:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:47:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_files    = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:68:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.value(params.busco_lineages ?: []),
          ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:114:37`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_prepared_genome.filter { meta, fasta -> params.blast_annotations == "all" || params.blast_annotations == "blastx" },
                                      ^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:114:43`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_prepared_genome.filter { meta, fasta -> params.blast_annotations == "all" || params.blast_annotations == "blastx" },
                                            ^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:198:32`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_multiqc_config        = Channel.fromPath(
                                 ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:203:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_config, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:204:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:207:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.fromPath(params.multiqc_logo, checkIfExists: true) :
          ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:208:9`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          Channel.empty()
          ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:211:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_workflow_summary     = Channel.value(paramsSummaryMultiqc(summary_params))
                                ^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:220:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_methods_description  = Channel.value(
                                ^^^^^^^
  ```
