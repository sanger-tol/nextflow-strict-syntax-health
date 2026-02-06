# Nextflow lint results

- Generated: 2026-02-06T13:21:24.479668+00:00
- Nextflow version: 25.12.0-edge
- Summary: 4 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/fastx_map_long_reads/main.nf:3:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/minimap2/index/main.nf'

    ```nextflow
    include { MINIMAP2_INDEX             } from '../../../modules/nf-core/minimap2/index/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fastx_map_long_reads/main.nf:68:5`: `MINIMAP2_INDEX` is not defined

    ```nextflow
        MINIMAP2_INDEX(ch_assemblies)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fastx_map_long_reads/main.nf:69:35`: `MINIMAP2_INDEX` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(MINIMAP2_INDEX.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fastx_map_long_reads/main.nf:76:18`: `MINIMAP2_INDEX` is not defined

    ```nextflow
            .combine(MINIMAP2_INDEX.out.index, by: 0)
                     ^^^^^^^^^^
    ```
