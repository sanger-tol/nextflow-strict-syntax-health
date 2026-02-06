# Nextflow lint results

- Generated: 2026-02-06T13:21:24.474325+00:00
- Nextflow version: 25.12.0-edge
- Summary: 10 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:1:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/faidx/main.nf'

    ```nextflow
    include { SAMTOOLS_FAIDX    } from '../../../modules/nf-core/samtools/faidx/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:2:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/merge/main.nf'

    ```nextflow
    include { SAMTOOLS_MERGE    } from '../../../modules/nf-core/samtools/merge/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:18:5`: `SAMTOOLS_FAIDX` is not defined

    ```nextflow
        SAMTOOLS_FAIDX(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:29:18`: `SAMTOOLS_FAIDX` is not defined

    ```nextflow
        ch_fai_gzi = SAMTOOLS_FAIDX.out.fai
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:30:15`: `SAMTOOLS_FAIDX` is not defined

    ```nextflow
            .join(SAMTOOLS_FAIDX.out.gzi, by: 0, remainder: true)
                  ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:68:9`: `SAMTOOLS_MERGE` is not defined

    ```nextflow
            SAMTOOLS_MERGE(
            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:75:26`: `SAMTOOLS_MERGE` is not defined

    ```nextflow
            ch_output_bam  = SAMTOOLS_MERGE.out.bam
                             ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:76:18`: `SAMTOOLS_MERGE` is not defined

    ```nextflow
                .mix(SAMTOOLS_MERGE.out.cram)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:78:27`: `SAMTOOLS_MERGE` is not defined

    ```nextflow
            ch_output_index = SAMTOOLS_MERGE.out.csi
                              ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/bam_samtools_merge_markdup/main.nf:79:18`: `SAMTOOLS_MERGE` is not defined

    ```nextflow
                .mix(SAMTOOLS_MERGE.out.crai)
                     ^^^^^^^^^^
    ```
