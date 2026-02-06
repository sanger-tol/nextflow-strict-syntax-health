# Nextflow lint results

- Generated: 2026-02-06T13:21:24.480345+00:00
- Nextflow version: 25.12.0-edge
- Summary: 28 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:2:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/busco/busco/main.nf'

    ```nextflow
    include { BUSCO_BUSCO         } from '../../../modules/nf-core/busco/busco/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:3:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/gfastats/main.nf'

    ```nextflow
    include { GFASTATS            } from '../../../modules/nf-core/gfastats/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:4:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/merquryfk/merquryfk/main.nf'

    ```nextflow
    include { MERQURYFK_MERQURYFK } from '../../../modules/nf-core/merquryfk/merquryfk/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:48:5`: `GFASTATS` is not defined

    ```nextflow
        GFASTATS(
        ^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:58:35`: `GFASTATS` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(GFASTATS.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:71:5`: `BUSCO_BUSCO` is not defined

    ```nextflow
        BUSCO_BUSCO(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:79:35`: `BUSCO_BUSCO` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(BUSCO_BUSCO.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:92:5`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
        MERQURYFK_MERQURYFK(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:103:14`: `GFASTATS` is not defined

    ```nextflow
            .mix(GFASTATS.out.assembly_summary)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:108:23`: `BUSCO_BUSCO` is not defined

    ```nextflow
        ch_busco_output = BUSCO_BUSCO.out.batch_summary
                          ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:109:14`: `BUSCO_BUSCO` is not defined

    ```nextflow
            .mix(BUSCO_BUSCO.out.short_summaries_txt)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:110:14`: `BUSCO_BUSCO` is not defined

    ```nextflow
            .mix(BUSCO_BUSCO.out.short_summaries_json)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:111:14`: `BUSCO_BUSCO` is not defined

    ```nextflow
            .mix(BUSCO_BUSCO.out.log)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:112:14`: `BUSCO_BUSCO` is not defined

    ```nextflow
            .mix(BUSCO_BUSCO.out.busco_dir)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:116:25`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
        ch_merqury_output = MERQURYFK_MERQURYFK.out.qv
                            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:117:14`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
            .mix(MERQURYFK_MERQURYFK.out.stats)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:118:14`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
            .mix(MERQURYFK_MERQURYFK.out.phased_block_stats)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:119:14`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
            .mix(MERQURYFK_MERQURYFK.out.images)
                 ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:126:32`: `GFASTATS` is not defined

    ```nextflow
        gfastats                 = GFASTATS.out.assembly_summary
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:128:32`: `BUSCO_BUSCO` is not defined

    ```nextflow
        busco_batch_summary      = BUSCO_BUSCO.out.batch_summary
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:129:32`: `BUSCO_BUSCO` is not defined

    ```nextflow
        busco_summary_txt        = BUSCO_BUSCO.out.short_summaries_txt
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:130:32`: `BUSCO_BUSCO` is not defined

    ```nextflow
        busco_summary_json       = BUSCO_BUSCO.out.short_summaries_json
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:131:32`: `BUSCO_BUSCO` is not defined

    ```nextflow
        busco_log                = BUSCO_BUSCO.out.log
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:132:32`: `BUSCO_BUSCO` is not defined

    ```nextflow
        busco_directory          = BUSCO_BUSCO.out.busco_dir
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:134:32`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
        merqury_qv               = MERQURYFK_MERQURYFK.out.qv
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:135:32`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
        merqury_completeness     = MERQURYFK_MERQURYFK.out.stats
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:136:32`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
        merqury_phased_stats     = MERQURYFK_MERQURYFK.out.phased_block_stats
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/genome_statistics/main.nf:137:32`: `MERQURYFK_MERQURYFK` is not defined

    ```nextflow
        merqury_images           = MERQURYFK_MERQURYFK.out.images
                                   ^^^^^^^^^^
    ```
