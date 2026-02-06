# Nextflow lint results

- Generated: 2026-02-06T13:21:24.481769+00:00
- Nextflow version: 25.12.0-edge
- Summary: 24 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:1:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/cooler/cload/main.nf'

    ```nextflow
    include { COOLER_CLOAD                               } from '../../../modules/nf-core/cooler/cload/main.nf'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:2:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/cooler/zoomify/main.nf'

    ```nextflow
    include { COOLER_ZOOMIFY                             } from '../../../modules/nf-core/cooler/zoomify/main.nf'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:3:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/gawk/main.nf'

    ```nextflow
    include { GAWK as GAWK_PROCESS_PAIRS_FILE            } from '../../../modules/nf-core/gawk/main.nf'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:4:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/juicertools/pre/main.nf'

    ```nextflow
    include { JUICERTOOLS_PRE                            } from '../../../modules/nf-core/juicertools/pre/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:5:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/pretextmap/main.nf'

    ```nextflow
    include { PRETEXTMAP                                 } from '../../../modules/nf-core/pretextmap/main.nf'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:6:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/pretextsnapshot/main.nf'

    ```nextflow
    include { PRETEXTSNAPSHOT                            } from '../../../modules/nf-core/pretextsnapshot/main.nf'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:23:5`: `PRETEXTMAP` is not defined

    ```nextflow
        PRETEXTMAP(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:31:5`: `PRETEXTSNAPSHOT` is not defined

    ```nextflow
        PRETEXTSNAPSHOT(PRETEXTMAP.out.pretext)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:31:21`: `PRETEXTMAP` is not defined

    ```nextflow
        PRETEXTSNAPSHOT(PRETEXTMAP.out.pretext)
                        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:32:35`: `PRETEXTSNAPSHOT` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(PRETEXTSNAPSHOT.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:45:5`: `COOLER_CLOAD` is not defined

    ```nextflow
        COOLER_CLOAD(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:51:35`: `COOLER_CLOAD` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(COOLER_CLOAD.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:56:5`: `COOLER_ZOOMIFY` is not defined

    ```nextflow
        COOLER_ZOOMIFY(COOLER_CLOAD.out.cool)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:56:20`: `COOLER_CLOAD` is not defined

    ```nextflow
        COOLER_ZOOMIFY(COOLER_CLOAD.out.cool)
                       ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:57:35`: `COOLER_ZOOMIFY` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(COOLER_ZOOMIFY.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:71:5`: `GAWK_PROCESS_PAIRS_FILE` is not defined

    ```nextflow
        GAWK_PROCESS_PAIRS_FILE(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:76:35`: `GAWK_PROCESS_PAIRS_FILE` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(GAWK_PROCESS_PAIRS_FILE.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:81:32`: `GAWK_PROCESS_PAIRS_FILE` is not defined

    ```nextflow
        ch_juicertools_pre_input = GAWK_PROCESS_PAIRS_FILE.out.output
                                   ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:88:5`: `JUICERTOOLS_PRE` is not defined

    ```nextflow
        JUICERTOOLS_PRE(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:92:35`: `JUICERTOOLS_PRE` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(JUICERTOOLS_PRE.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:95:19`: `PRETEXTMAP` is not defined

    ```nextflow
        pretext     = PRETEXTMAP.out.pretext
                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:96:19`: `PRETEXTSNAPSHOT` is not defined

    ```nextflow
        pretext_png = PRETEXTSNAPSHOT.out.image
                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:97:19`: `COOLER_ZOOMIFY` is not defined

    ```nextflow
        cool        = COOLER_ZOOMIFY.out.mcool
                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/pairs_create_contact_maps/main.nf:98:19`: `JUICERTOOLS_PRE` is not defined

    ```nextflow
        hic         = JUICERTOOLS_PRE.out.hic
                      ^^^^^^^^^^
    ```
