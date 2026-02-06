# Nextflow lint results

- Generated: 2026-02-06T13:21:24.482950+00:00
- Nextflow version: 25.12.0-edge
- Summary: 4 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/telo_finder/main.nf:5:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/gawk/main.nf'

    ```nextflow
    include { GAWK                      } from '../../../modules/nf-core/gawk/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/telo_finder/main.nf:40:9`: `GAWK` is not defined

    ```nextflow
            GAWK (
            ^^^^^^
    ```

- Error: `subworkflows/sanger-tol/telo_finder/main.nf:45:43`: `GAWK` is not defined

    ```nextflow
            ch_versions     = ch_versions.mix(GAWK.out.versions)
                                              ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/telo_finder/main.nf:56:37`: `GAWK` is not defined

    ```nextflow
            ch_regions_for_extraction = GAWK.out.output
                                        ^^^^^^^^^^
    ```
