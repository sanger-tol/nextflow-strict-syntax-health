# Nextflow lint results

- Generated: 2026-02-06T13:21:24.473282+00:00
- Nextflow version: 25.12.0-edge
- Summary: 3 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/ancestral_annotation/main.nf:4:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/faidx/main.nf'

    ```nextflow
    include { SAMTOOLS_FAIDX        } from '../../../modules/nf-core/samtools/faidx/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/ancestral_annotation/main.nf:32:5`: `SAMTOOLS_FAIDX` is not defined

    ```nextflow
        SAMTOOLS_FAIDX(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/ancestral_annotation/main.nf:44:9`: `SAMTOOLS_FAIDX` is not defined

    ```nextflow
            SAMTOOLS_FAIDX.out.fai
            ^^^^^^^^^^
    ```
