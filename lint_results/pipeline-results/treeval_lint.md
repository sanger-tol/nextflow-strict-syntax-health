# Nextflow lint results

- Generated: 2026-02-06T13:21:03.105285739Z
- Nextflow version: 25.12.0-edge
- Summary: 21 errors, 177 warnings

## :x: Errors

- Error: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:44:9`: `base` is already declared

  ```nextflow
      def base    = "45022_3#2"
          ^^^^
  ```

- Error: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:45:9`: `chunkid` is already declared

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

- Error: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:56:20`: `VERSION` is not defined

  ```nextflow
          staden_io: $VERSION
                     ^^^^^^^^
  ```

- Error: `modules/local/get/largest_scaffold/main.nf:15:9`: `largest_scaff` is not defined

  ```nextflow
      env largest_scaff   , emit: scaff_size
          ^^^^^^^^^^^^^
  ```

- Error: `modules/nf-core/pretextsnapshot/main.nf:45:26`: `VERSION` is not defined

  ```nextflow
          pretextsnapshot: $VERSION
                           ^^^^^^^^
  ```

- Error: `modules/nf-core/samtools/view/main.nf:66:9`: `index` is already declared

  ```nextflow
      def index = args.contains("--write-index") ? "touch ${prefix}.${file_type}.csi" : ""
          ^^^^^
  ```

- Error: `modules/nf-core/yahs/main.nf:42:13`: `prefix` is not defined

  ```nextflow
      touch ${prefix}_scaffold_final.fa
              ^^^^^^
  ```

- Error: `modules/nf-core/yahs/main.nf:43:13`: `prefix` is not defined

  ```nextflow
      touch ${prefix}_scaffolds_final.agp
              ^^^^^^
  ```

- Error: `modules/nf-core/yahs/main.nf:44:13`: `prefix` is not defined

  ```nextflow
      touch ${prefix}.bin
              ^^^^^^
  ```

- Error: `subworkflows/local/generate_genome/main.nf:31:30`: `map_order` is already declared

  ```nextflow
          .map{ ref_meta, ref, map_order ->
                               ^^^^^^^^^
  ```

- Error: `subworkflows/local/hic_mapping/main.nf:61:37`: `hic_reads_path` is already declared

  ```nextflow
          .map { meta, ref, hic_meta, hic_reads_path ->
                                      ^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/hic_mapping/main.nf:166:21`: Variables in a closure should be declared with `def`

  ```nextflow
                      new_location = file(copy_to_dir).mkdirs()
                      ^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/insilico_digest/main.nf:41:27`: `reference` is already declared

  ```nextflow
          .multiMap { meta, reference, enzyme_id ->
                            ^^^^^^^^^
  ```

- Error: `subworkflows/local/kmer/main.nf:29:22`: `reads_path` is already declared

  ```nextflow
          .map { meta, reads_path ->
                       ^^^^^^^^^^
  ```

- Error: `subworkflows/local/pep_alignments/main.nf:3:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import java.math.RoundingMode;
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pep_alignments/main.nf:4:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import java.math.BigDecimal;
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/synteny/main.nf:31:41`: `class` is not allowed as an identifier because it is a Groovy keyword

  ```nextflow
                                          class: meta.class,
                                          ^^^^^
  ```

- Error: `subworkflows/local/telo_finder/main.nf:64:29`: Variables in a closure should be declared with `def`

  ```nextflow
                              new_meta = meta + [direction: 5]
                              ^^^^^^^^
  ```

- Error: `subworkflows/local/yaml_input/main.nf:25:21`: `class` is not allowed as an identifier because it is a Groovy keyword

  ```nextflow
                      class: data.assembly.defined_class,
                      ^^^^^
  ```

## :warning: Warnings

- Warning: `main.nf:29:5`: Params should be declared at the top-level (i.e. outside the workflow)

  ```nextflow
      params.mode      = params.mode ?: "FULL"
      ^^^^^^
  ```

- Warning: `main.nf:30:5`: Params should be declared at the top-level (i.e. outside the workflow)

  ```nextflow
      params.binfile   = params.binfile ?: false
      ^^^^^^
  ```

- Warning: `main.nf:31:5`: Params should be declared at the top-level (i.e. outside the workflow)

  ```nextflow
      params.juicer    = params.juicer ?: false
      ^^^^^^
  ```

- Warning: `main.nf:32:5`: Params should be declared at the top-level (i.e. outside the workflow)

  ```nextflow
      params.run_hires = params.run_hires ?: true
      ^^^^^^
  ```

- Warning: `modules/local/assign/ancestral/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ''
          ^^^^
  ```

- Warning: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/cram/filter_align_bwamem2_fixmate_sort/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^
  ```

- Warning: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:20:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:31:11`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          ${projectDir}/bin/grep_pg.sh |  \\
            ^^^^^^^^^^
  ```

- Warning: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:32:16`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          perl ${projectDir}/bin/filter_five_end.pl |  \\
                 ^^^^^^^^^^
  ```

- Warning: `modules/local/cram/filter_minimap2_filter5end_fixmate_sort/main.nf:33:11`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          ${projectDir}/bin/awk_filter_reads.sh |  \\
            ^^^^^^^^^^
  ```

- Warning: `modules/local/extract/ancestral/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ''
          ^^^^
  ```

- Warning: `modules/local/extract/ancestral/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def prefix  = task.ext.prefix   ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/find/half_coverage/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ''
          ^^^^
  ```

- Warning: `modules/local/find/telomere_regions/main.nf:17:9`: Variable was declared but not used

  ```nextflow
      def VERSION = "1.0" // WARN: Version information not provided by tool on CLI. Please update this string when bumping container versions.
          ^^^^^^^
  ```

- Warning: `modules/local/find/telomere_regions/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def find_telomere = task.ext.find_telomere ?: ''
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/local/find/telomere_regions/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def VERSION = "1.0" // WARN: Version information not provided by tool on CLI. Please update this string when bumping container versions.
          ^^^^^^^
  ```

- Warning: `modules/local/find/telomere_regions/main.nf:31:9`: Variable was declared but not used

  ```nextflow
      def find_telomere = task.ext.find_telomere ?: ''
          ^^^^^^^^^^^^^
  ```

- Warning: `modules/local/find/telomere_windows/main.nf:25:39`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
      java ${telomere_jvm_params} -cp ${projectDir}/bin/${telomere_jar} FindTelomereWindows $file $telomere_window_cut > ${prefix}.windows
                                        ^^^^^^^^^^
  ```

- Warning: `modules/local/find/telomere_windows/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def telomere = task.ext.telomere ?: ''
          ^^^^^^^^
  ```

- Warning: `modules/local/get/largest_scaffold/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def prefix      = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/local/get/paired_contact_bed/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def pulled = '-T sort_tmp'
          ^^^^^^
  ```

- Warning: `modules/local/graph/overall_coverage/main.nf:21:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/juicer/tools_pre/main.nf:30:16`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          -jar ${projectDir}/bin/${juicer_tools_jar} pre \\
                 ^^^^^^^^^^
  ```

- Warning: `modules/local/juicer/tools_pre/main.nf:37:59`: The use of `projectDir` in a process is discouraged -- input files should be provided as process inputs

  ```nextflow
          juicer tools: \$(java ${juicer_jvm_params} -jar ${projectDir}/bin/${juicer_tools_jar} -V | grep "Juicer Tools Version" | sed 's/Juicer Tools Version //')
                                                            ^^^^^^^^^^
  ```

- Warning: `modules/local/makecmap/cmap2bed/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/selfcomp/mapids/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/selfcomp/mapids/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/selfcomp/mummer2bed/main.nf:35:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/selfcomp/splitfasta/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/selfcomp/splitfasta/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def args        = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/local/subsample/bam/main.nf:18:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
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

- Warning: `modules/nf-core/custom/dumpsoftwareversions/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/custom/getchromsizes/main.nf:24:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
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

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:42:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def mat_ktab = matktab ? "${matktab.find{ it.toString().endsWith(".ktab") }}" : ''
                                                ^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:43:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def pat_ktab = patktab ? "${patktab.find{ it.toString().endsWith(".ktab") }}" : ''
                                                ^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:50:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ${fastk_ktab.find{ it.toString().endsWith(".ktab") }} \\
                             ^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:33:9`: Variable was declared but not used

  ```nextflow
      def args2 = task.ext.args2 ?: ''
          ^^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:37:9`: Variable was declared but not used

  ```nextflow
      def bam_index = bam_index_extension ? "${prefix}.bam##idx##${prefix}.bam.${bam_index_extension} --write-index" : "${prefix}.bam"
          ^^^^^^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:70:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/paftools/sam2paf/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ""
          ^^^^
  ```

- Warning: `modules/nf-core/ucsc/bedgraphtobigwig/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/ancestral_gene/main.nf:19:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/ancestral_gene/main.nf:53:25`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dot_genome.map{ it[1] },      // Pull file from tuple(meta, file)
                          ^^
  ```

- Warning: `subworkflows/local/busco_annotation/main.nf:31:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions                 = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/busco_annotation/main.nf:85:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dot_genome.map{it[1]},      // Gets file from tuple (meta, file)
                         ^^
  ```

- Warning: `subworkflows/local/gap_finder/main.nf:15:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:23:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      as_files            // Channel: [ val(meta), path(file) ]
      ^^^^^^^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:26:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:29:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, file ->
                      ^^^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:32:16`: Variable was declared but not used

  ```nextflow
          .set { assembly_class }
                 ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:65:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              pep: it[0].type  == 'pep'
                   ^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:66:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              gen: it[0].type  == 'cdna'
                   ^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:67:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              rna: it[0].type  == 'rna'
                   ^^
  ```

- Warning: `subworkflows/local/gene_alignment/main.nf:68:18`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              cds: it[0].type  == 'cds'
                   ^^
  ```

- Warning: `subworkflows/local/generate_genome/main.nf:20:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_genome/main.nf:21:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genomesize   = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_genome/main.nf:22:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_fai   = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_genome/main.nf:40:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              sorted      : it[0].map_order == "length"
                            ^^
  ```

- Warning: `subworkflows/local/generate_genome/main.nf:41:27`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              unsorted    : it[0].map_order != "length"
                            ^^
  ```

- Warning: `subworkflows/local/generate_sorted_genome/main.nf:14:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_sorted_genome/main.nf:15:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      genome_size     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_unsorted_genome/main.nf:13:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_unsorted_genome/main.nf:14:5`: Variable was declared but not used

  ```nextflow
      genome_size     = Channel.empty()
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/generate_unsorted_genome/main.nf:14:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      genome_size     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_bamtobed/main.nf:22:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:22:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:23:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      mappedbam_ch        = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:34:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ cram_id, cram_info, ref_id, ref_dir, bwa_id, bwa_path ->
                                    ^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:34:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ cram_id, cram_info, ref_id, ref_dir, bwa_id, bwa_path ->
                                                     ^^^^^^
  ```

- Warning: `subworkflows/local/hic_bwamem2/main.nf:65:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, file ->
                ^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:37:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      assembly_id         // Channel: val( id )
      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:45:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      run_hires           // boolean: Generate high resolution pretext maps
      ^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:48:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:53:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_cool_bin         = Channel.of( 1000 )
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:61:22`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, ref, hic_meta, hic_reads_path ->
                       ^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:61:27`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, ref, hic_meta, hic_reads_path ->
                            ^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:83:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, hic_read_path, ref_meta, ref ->
                      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:90:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              minimap2      : it[0].aligner == "minimap2"
                              ^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:91:29`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              bwamem2       : it[0].aligner == "bwamem2"
                              ^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:126:54`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { bam_meta, bam, ref_meta, ref_fa, genome_meta, genome_file ->
                                                       ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:152:31`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { ref_meta, ref, fai_meta, fai ->
                                ^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:166:21`: Variable was declared but not used

  ```nextflow
                      new_location = file(copy_to_dir).mkdirs()
                      ^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:244:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          hires_pretext       = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:317:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .multiMap {  meta, paired_contacts, meta_my_genome, my_genome ->
                                                  ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:373:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, pairs, bed, cool_bin, meta_my_genome, my_genome ->
                                                  ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/hic_mapping/main.nf:394:28`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, cools, cool_bin ->
                             ^^^^^^^^
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

- Warning: `subworkflows/local/hic_minimap2/main.nf:42:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ cram_id, cram_info, ref_id, ref_dir, mmi_id, mmi_path->
                                    ^^^^^^
  ```

- Warning: `subworkflows/local/hic_minimap2/main.nf:42:52`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ cram_id, cram_info, ref_id, ref_dir, mmi_id, mmi_path->
                                                     ^^^^^^
  ```

- Warning: `subworkflows/local/hic_minimap2/main.nf:74:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, file ->
                ^^^^
  ```

- Warning: `subworkflows/local/insilico_digest/main.nf:23:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/insilico_digest/main.nf:63:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, cfile  ->
                ^^^^
  ```

- Warning: `subworkflows/local/insilico_digest/main.nf:120:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, bed, meta_2, dot_genome, as_file ->
                                 ^^^^^^
  ```

- Warning: `subworkflows/local/kmer/main.nf:23:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/kmer/main.nf:58:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta_hist, hist, meta_ktab, ktab, meta_ref, primary ->
                                 ^^^^^^^^^
  ```

- Warning: `subworkflows/local/kmer/main.nf:58:49`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta_hist, hist, meta_ktab, ktab, meta_ref, primary ->
                                                  ^^^^^^^^
  ```

- Warning: `subworkflows/local/nuc_alignments/main.nf:28:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/nuc_alignments/main.nf:39:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, nuc_file, ref_meta, ref, intron ->
                                 ^^^^^^^^
  ```

- Warning: `subworkflows/local/nuc_alignments/main.nf:155:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[0].file_size >= 141 } // Take the first item in input (meta) and check if size is more than a symlink
                    ^^
  ```

- Warning: `subworkflows/local/nuc_alignments/main.nf:157:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, ref, genome_meta, genome ->
                                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pep_alignments/main.nf:22:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/pep_alignments/main.nf:39:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { pep_meta, pep_file, miniprot_meta, miniprot_index ->
                                          ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/punchlist/main.nf:11:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      reference_tuple // Channel: tuple [ val(meta), path(reference)]
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/punchlist/main.nf:15:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:27:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions                 = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:33:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, files ->
                 ^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:45:50`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, ref, reads_path, read_meta, readfolder ->
                                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:63:90`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, reads_path, ref, bam_output, cigar_paf, cigar_bam, bed_output, reads_type ->
                                                                                           ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:90:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, file ->
                 ^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:124:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, my_genome_meta, my_genome ->
                                  ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:188:5`: Variable was declared but not used

  ```nextflow
      ch_depthgraph           = GRAPH_OVERALL_COVERAGE.out.part
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:196:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_depthgraph, depthgraph, meta_my_genome, my_genome ->
                                  ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:196:62`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_depthgraph, depthgraph, meta_my_genome, my_genome ->
                                                               ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:219:21`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_my_genome, my_genome, ref_meta, ref ->
                      ^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:219:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_my_genome, my_genome, ref_meta, ref ->
                                  ^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/read_coverage/main.nf:219:70`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, file, meta_my_genome, my_genome, ref_meta, ref ->
                                                                       ^^^
  ```

- Warning: `subworkflows/local/repeat_density/main.nf:28:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/repeat_density/main.nf:67:35`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, windows_file, repeat_meta, repeat_file ->
                                    ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/repeat_density/main.nf:137:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ intersect_meta, bed, sorted_meta, windows_file ->
                                     ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/repeat_density/main.nf:170:37`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          GNU_SORT_B.out.sorted.map { it[1] } // Pulls file from tuple of meta and file
                                      ^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:45:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions             = Channel.empty()
                                ^^^^^^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:62:12`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { it, file ->
             ^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:86:12`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { it, file ->
             ^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:120:12`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, myfiles ->
             ^^^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:127:12`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      .map { meta, myfiles ->
             ^^^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:157:15`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map{ meta, file ->
                ^^^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:163:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { files, meta, ref ->
                              ^^^
  ```

- Warning: `subworkflows/local/selfcomp/main.nf:247:24`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          dot_genome.map{it[1]}, // Pulls file from tuple ( meta and file )
                         ^^
  ```

- Warning: `subworkflows/local/synteny/main.nf:14:35`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions                 = Channel.empty()
                                    ^^^^^^^
  ```

- Warning: `subworkflows/local/telo_extraction/main.nf:12:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/telo_extraction/main.nf:25:47`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def safe_windows = windows_file.ifEmpty { Channel.empty() }
                                                ^^^^^^^
  ```

- Warning: `subworkflows/local/telo_extraction/main.nf:46:57`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_gawk_output  = GAWK_MAP_TELO.out.output.ifEmpty( Channel.empty() )
                                                          ^^^^^^^
  ```

- Warning: `subworkflows/local/telo_finder/main.nf:18:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_treeval_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:10:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:12:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel.value(input_file)
      ^^^^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:68:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, file ->
                    ^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:86:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      unzipped_input = Channel.empty()
                       ^^^^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:97:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_assem_reads    = parsed.read_ch.filter { it } // filter []
                                                  ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:101:50`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_align_genesets = parsed.genesets.filter { it } // filter []
                                                   ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:102:49`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_synteny_paths  = parsed.synteny.filter { it } // filter []
                                                  ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:103:53`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      ch_intron_size    = parsed.intron_size.filter { it } // filter ""
                                                      ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:114:64`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  def fn_get_validated_channel (data_type, tolid_ver, read_type, defined_class, project_id, files_list) {
                                                                 ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:114:79`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
  def fn_get_validated_channel (data_type, tolid_ver, read_type, defined_class, project_id, files_list) {
                                                                                ^^^^^^^^^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:127:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .collect { it.trim() }
                             ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:128:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .findAll { it } // Remove empty lines
                             ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:141:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              !it.toString().contains(".cram")
               ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:148:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              !it.toString().contains(".fasta.gz") &&
               ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:149:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              !it.toString().contains(".fa.gz") &&
               ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:150:14`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              !it.toString().contains(".fn.gz")
               ^^
  ```

- Warning: `subworkflows/local/yaml_input/main.nf:175:34`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          all_files.collect { file(it, checkIfExists: true) }
                                   ^^
  ```

- Warning: `workflows/treeval.nf:58:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      kmer_prof_file  // channel:
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/treeval.nf:60:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      supp_reads      // channel:
      ^^^^^^^^^^
  ```

- Warning: `workflows/treeval.nf:80:98`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      exclude_steps_list      = params.steps == "NONE" ? [] : params.steps.tokenize(',').collect { it.trim() }
                                                                                                   ^^
  ```

- Warning: `workflows/treeval.nf:129:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:139:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:143:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:147:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:151:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:183:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_enzyme       = Channel.of( "bspq1","bsss1","DLE1" )
                            ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:233:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_repeat_density   = Channel.of([[],[]])
                                ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:247:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_gap_file         = Channel.of([[],[]])
                                ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:290:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_coverage_bg_norm = Channel.of([[],[]])
                                ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:306:31`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
          ch_telo_bedgraph    = Channel.of([])
                                ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:363:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:387:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```
