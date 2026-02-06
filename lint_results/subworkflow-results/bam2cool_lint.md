# Nextflow lint results

- Generated: 2026-02-06T13:21:24.473585+00:00
- Nextflow version: 25.12.0-edge
- Summary: 13 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:4:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/cooler/cload/main.nf'

    ```nextflow
    include { COOLER_CLOAD              } from '../../../modules/nf-core/cooler/cload/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:5:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/cooler/merge/main.nf'

    ```nextflow
    include { COOLER_MERGE              } from '../../../modules/nf-core/cooler/merge/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:6:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/cooler/zoomify/main.nf'

    ```nextflow
    include { COOLER_ZOOMIFY            } from '../../../modules/nf-core/cooler/zoomify/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:65:5`: `COOLER_CLOAD` is not defined

    ```nextflow
        COOLER_CLOAD(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:71:35`: `COOLER_CLOAD` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(COOLER_CLOAD.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:76:31`: `COOLER_CLOAD` is not defined

    ```nextflow
        ch_cool_files_for_merge = COOLER_CLOAD.out.cool
                                  ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:84:5`: `COOLER_MERGE` is not defined

    ```nextflow
        COOLER_MERGE(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:87:35`: `COOLER_MERGE` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(COOLER_MERGE.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:92:5`: `COOLER_ZOOMIFY` is not defined

    ```nextflow
        COOLER_ZOOMIFY(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:93:9`: `COOLER_MERGE` is not defined

    ```nextflow
            COOLER_MERGE.out.cool
            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:95:35`: `COOLER_ZOOMIFY` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(COOLER_ZOOMIFY.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:101:23`: `COOLER_MERGE` is not defined

    ```nextflow
        merged_cool     = COOLER_MERGE.out.cool
                          ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam2cool/main.nf:102:23`: `COOLER_ZOOMIFY` is not defined

    ```nextflow
        mcool           = COOLER_ZOOMIFY.out.mcool
                          ^^^^^^^^^^
    ```
