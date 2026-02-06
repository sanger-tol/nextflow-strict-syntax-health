# Nextflow lint results

- Generated: 2026-02-06T13:21:09.759481758Z
- Nextflow version: 25.12.0-edge
- Summary: 11 errors, 53 warnings

## :x: Errors

- Error: `conf/modules.config:17:17`: Unexpected input: ':'

    ```nextflow
            withName: '.*:ALIGN_PACBIO:FILTER_PACBIO:SAMTOOLS_CONVERT' {
                    ^
    ```

- Error: `main.nf:16:1`: Module could not be parsed: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/pipelines/variantcalling/workflows/variantcalling.nf'

    ```nextflow
    include { VARIANTCALLING          } from './workflows/variantcalling'
    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Error: `main.nf:42:5`: `VARIANTCALLING` is not defined

    ```nextflow
        VARIANTCALLING (
        ^^^^^^^^^^^^^^
    ```

- Error: `subworkflows/local/deepvariant_caller.nf:41:68`: `fasta` is already declared

    ```nextflow
        fai = reads_fasta.map{ meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fai ] }
                                                                       ^^^^^
    ```

- Error: `subworkflows/local/deepvariant_caller.nf:90:26`: `vcf` is already declared

    ```nextflow
            .map { meta_vcf, vcf, meta -> [ meta_vcf + meta, vcf ] }
                             ^^^
    ```

- Error: `subworkflows/local/deepvariant_caller.nf:91:25`: `vcf` is already declared

    ```nextflow
            .branch { meta, vcf ->
                            ^^^
    ```

- Error: `subworkflows/local/filter_pacbio.nf:51:12`: `db` is already declared

    ```nextflow
        db.map{db -> [ [], db]}.set{ch_db}
               ^^
    ```

- Error: `subworkflows/local/input_filter_split.nf:63:34`: `fasta` is already declared

    ```nextflow
        ch_fasta = fasta.map { meta, fasta -> [ [ 'id': fasta.baseName ], fasta ] }.first()
                                     ^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:223:13`: `platform` was assigned but not declared

    ```nextflow
                platform = "PACBIO"
                ^^^^^^^^
    ```

- Error: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:225:122`: `platform` is not defined

    ```nextflow
            meta.read_group  = "\'@RG\\tID:" + datafile.toString().split('/')[-1].split('\\.')[0..-2].join('.') + "\\tPL:" + platform + "\\tSM:" + meta.sample + "\'"
                                                                                                                             ^^^^^^^^
    ```

- Error: `workflows/variantcalling.nf:224:23`: Unexpected input: '\n'

    ```nextflow
            n_sequences ++
                          ^
    ```


## :warning: Warnings

- Warning: `modules/nf-core/bcftools/index/main.nf:23:9`: Variable was declared but not used

    ```nextflow
        def prefix = task.ext.prefix ?: "${meta.id}"
            ^^^^^^
    ```

- Warning: `modules/nf-core/bcftools/index/main.nf:40:9`: Variable was declared but not used

    ```nextflow
        def prefix = task.ext.prefix ?: "${meta.id}"
            ^^^^^^
    ```

- Warning: `modules/nf-core/blast/blastn/main.nf:52:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/deepvariant/vcfstatsreport/main.nf:25:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/gunzip/main.nf:43:9`: Variable was declared but not used

    ```nextflow
        def args        = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

    ```nextflow
        def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
            ^^^^^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:97:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--bed') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:98:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--exclude-bed') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:99:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--hapcount') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:100:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--positions') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:101:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--exclude-positions') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:106:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--diff') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:107:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--gzdiff') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:108:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--diff-bcf') }
                             ^^
    ```

- Warning: `subworkflows/local/align_pacbio.nf:19:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/convert_stats.nf:18:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:20:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:23:53`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | map { meta, cram, crai, interval, meta_fasta, fasta, fai ->
                                                        ^^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:23:60`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | map { meta, cram, crai, interval, meta_fasta, fasta, fai ->
                                                               ^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:38:31`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fasta = reads_fasta.map { meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fasta ] }
                                  ^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:38:37`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fasta = reads_fasta.map { meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fasta ] }
                                        ^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:38:43`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fasta = reads_fasta.map { meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fasta ] }
                                              ^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:38:49`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fasta = reads_fasta.map { meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fasta ] }
                                                    ^^^^^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:38:78`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fasta = reads_fasta.map { meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fasta ] }
                                                                                 ^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:41:28`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fai = reads_fasta.map{ meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fai ] }
                               ^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:41:34`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fai = reads_fasta.map{ meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fai ] }
                                     ^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:41:40`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fai = reads_fasta.map{ meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fai ] }
                                           ^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:41:46`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fai = reads_fasta.map{ meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fai ] }
                                                 ^^^^^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:41:68`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        fai = reads_fasta.map{ meta, cram, crai, interval, meta_fasta, fasta, fai -> [ meta_fasta, fai ] }
                                                                       ^^^^^
    ```

- Warning: `subworkflows/local/deepvariant_caller.nf:91:25`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .branch { meta, vcf ->
                            ^^^
    ```

- Warning: `subworkflows/local/filter_pacbio.nf:23:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/filter_pacbio.nf:68:29`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | map { meta, bam, csi, list -> [meta, bam, csi] }
                                ^^^^
    ```

- Warning: `subworkflows/local/filter_pacbio.nf:72:13`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | map { meta, bam, csi, list -> list }
                ^^^^
    ```

- Warning: `subworkflows/local/filter_pacbio.nf:72:19`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | map { meta, bam, csi, list -> list }
                      ^^^
    ```

- Warning: `subworkflows/local/filter_pacbio.nf:72:24`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | map { meta, bam, csi, list -> list }
                           ^^^
    ```

- Warning: `subworkflows/local/input_filter_split.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/input_filter_split.nf:23:16`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | branch { meta, fa ->
                   ^^^^
    ```

- Warning: `subworkflows/local/input_filter_split.nf:46:13`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        | map { meta, fastas -> fastas }
                ^^^^
    ```

- Warning: `subworkflows/local/input_filter_split.nf:63:28`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        ch_fasta = fasta.map { meta, fasta -> [ [ 'id': fasta.baseName ], fasta ] }.first()
                               ^^^^
    ```

- Warning: `subworkflows/local/input_merge.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/input_merge.nf:19:21`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .map{ meta, bam_cram -> [ meta.sample, meta ] }
                        ^^^^^^^^
    ```

- Warning: `subworkflows/local/process_vcf.nf:14:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs   // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        input             //  string: Path to input samplesheet
        ^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:41:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        interval
        ^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:115:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_fasta = Channel.fromPath(fasta)
                   ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:125:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
            ch_fai = Channel.fromPath(fai)
                     ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:127:18`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
            ch_fai = Channel.empty()
                     ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:130:41`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        if (params.interval){ ch_interval = Channel.fromPath(params.interval) } else { ch_interval = Channel.empty() }
                                            ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:130:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        if (params.interval){ ch_interval = Channel.fromPath(params.interval) } else { ch_interval = Channel.empty() }
                                                                                                     ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:135:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
            ch_positions = Channel.fromPath(include_positions)
                           ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:137:24`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
            ch_positions = Channel.fromPath(exclude_positions)
                           ^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcalling_pipeline/main.nf:218:76`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
            if ( !datafile || !validFormats.any { datafile.toString().endsWith(it) } ) {
                                                                               ^^
    ```
