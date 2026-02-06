# Nextflow lint results

- Generated: 2026-02-06T13:21:24.479985+00:00
- Nextflow version: 25.12.0-edge
- Summary: 7 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/gap_finder/main.nf:5:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/seqtk/cutn/main.nf'

    ```nextflow
    include { SEQTK_CUTN    } from '../../../modules/nf-core/seqtk/cutn/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/gap_finder/main.nf:6:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/gawk/main.nf'

    ```nextflow
    include { GAWK          } from '../../../modules/nf-core/gawk/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/gap_finder/main.nf:19:5`: `SEQTK_CUTN` is not defined

    ```nextflow
        SEQTK_CUTN (
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/gap_finder/main.nf:27:5`: `GAWK` is not defined

    ```nextflow
        GAWK (
        ^^^^^^
    ```

- Error: `subworkflows/sanger-tol/gap_finder/main.nf:28:9`: `SEQTK_CUTN` is not defined

    ```nextflow
            SEQTK_CUTN.out.bed,
            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/gap_finder/main.nf:32:40`: `GAWK` is not defined

    ```nextflow
        ch_versions     = ch_versions.mix( GAWK.out.versions )
                                           ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/gap_finder/main.nf:36:23`: `GAWK` is not defined

    ```nextflow
        gap_file        = GAWK.out.output
                          ^^^^^^^^^^
    ```
