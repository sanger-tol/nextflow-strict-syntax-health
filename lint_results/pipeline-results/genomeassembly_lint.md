# Nextflow lint results

- Generated: 2026-02-06T13:19:18.432854596Z
- Nextflow version: 25.12.0-edge
- Summary: 5 errors, 31 warnings

## :x: Errors

- Error: `conf/base.config:112:17`: Unexpected input: 'reference'

    ```nextflow
                    reference.size())
                    ^
    ```

- Error: `conf/longranger_lsf_sanger.config:26:28`: `LSF_BINDIR` is not defined (hint: use `env('...')` to access environment variable)

    ```nextflow
            "--env APPEND_PATH=$LSF_BINDIR:$LSF_SERVERDIR:/software/singularity/3.11.4/bin"
                               ^^^^^^^^^^^
    ```

- Error: `conf/longranger_lsf_sanger.config:26:40`: `LSF_SERVERDIR` is not defined (hint: use `env('...')` to access environment variable)

    ```nextflow
            "--env APPEND_PATH=$LSF_BINDIR:$LSF_SERVERDIR:/software/singularity/3.11.4/bin"
                                           ^^^^^^^^^^^^^^
    ```

- Error: `conf/modules.config:41:13`: `hapdir` was assigned but not declared

    ```nextflow
                hapdir = meta._hap ?: "hap1"
                ^^^^^^
    ```

- Error: `conf/modules.config:42:42`: `hapdir` is not defined

    ```nextflow
                subdir_name = "scaffolding_${hapdir}/yahs/"
                                             ^^^^^^
    ```


## :warning: Warnings

- Warning: `modules/nf-core/bcftools/consensus/main.nf:40:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/bcftools/consensus/main.nf:42:9`: Variable was declared but not used

    ```nextflow
        def masking = mask ? "-m $mask" : ""
            ^^^^^^^
    ```

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

- Warning: `modules/nf-core/gatk4/mergevcfs/main.nf:25:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        def input_list = vcf.collect{ "--INPUT $it"}.join(' ')
                                               ^^
    ```

- Warning: `modules/nf-core/genomescope2/main.nf:47:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:27:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        input_mat       = matktab   ? "${matktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}"   : ''
                                                       ^^
    ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:28:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        input_pat       = patktab   ? "${patktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}"   : ''
                                                       ^^
    ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:29:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        def input_child = childktab ? "${childktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}" : ''
                                                         ^^
    ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:51:9`: Variable was declared but not used

    ```nextflow
        def args  = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:52:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        input_mat = matktab ? "${matktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}" : ''
                                               ^^
    ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:53:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        input_pat = patktab ? "${patktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}" : ''
                                               ^^
    ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:45:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        fk_ktab     = fastk_ktab ? "${fastk_ktab.find{ it.toString().endsWith(".ktab") }}" : ''
                                                       ^^
    ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:46:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        mat_hapktab = mathaptab  ? "${mathaptab.find{ it.toString().endsWith(".ktab") }}"  : ''
                                                      ^^
    ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:47:51`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        pat_hapktab = pathaptab  ? "${pathaptab.find{ it.toString().endsWith(".ktab") }}"  : ''
                                                      ^^
    ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

    ```nextflow
        def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
            ^^^^^^
    ```

- Warning: `modules/nf-core/seqkit/grep/main.nf:46:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/yak/count/main.nf:39:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/sanger-tol/samtools/mergedup/main.nf:56:9`: Variable was declared but not used

    ```nextflow
        def args      = task.ext.args  ?: ''
            ^^^^
    ```

- Warning: `subworkflows/local/raw_assembly/main.nf:95:19`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .filter { meta, asm ->
                      ^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_genomeassembly_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs   // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/bam_stats_samtools/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:25:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `workflows/genomeassembly.nf:107:39`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .multiMap { meta, hap1, hap2, meta_reads, reads ->
                                          ^^^^^^^^^^
    ```

- Warning: `workflows/genomeassembly.nf:169:15`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_haps = Channel.of("hap1", "hap2")
                  ^^^^^^^
    ```

- Warning: `workflows/genomeassembly.nf:256:19`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .filter { meta, asm -> asm }
                      ^^^^
    ```

- Warning: `workflows/genomeassembly.nf:292:26`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
                .map { meta, reads -> [meta, meta.species] }
                             ^^^^^
    ```

- Warning: `workflows/genomeassembly.nf:309:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        def topic_versions = Channel.topic("versions")
                             ^^^^^^^
    ```

- Warning: `workflows/genomeassembly.nf:333:17`: Variable was declared but not used

    ```nextflow
            ).set { ch_collated_versions }
                    ^^^^^^^^^^^^^^^^^^^^
    ```
