# Nextflow lint results

- Generated: 2026-02-06T13:21:24.476513+00:00
- Nextflow version: 25.12.0-edge
- Summary: 20 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:2:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/faidx/main.nf'

    ```nextflow
    include { SAMTOOLS_FAIDX as SAMTOOLS_FAIDX_CONTIGS   } from '../../../modules/nf-core/samtools/faidx/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:3:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/faidx/main.nf'

    ```nextflow
    include { SAMTOOLS_FAIDX as SAMTOOLS_FAIDX_SCAFFOLDS } from '../../../modules/nf-core/samtools/faidx/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:4:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/yahs/main.nf'

    ```nextflow
    include { YAHS                                       } from '../../../modules/nf-core/yahs/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:31:5`: `SAMTOOLS_FAIDX_CONTIGS` is not defined

    ```nextflow
        SAMTOOLS_FAIDX_CONTIGS(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:41:18`: `SAMTOOLS_FAIDX_CONTIGS` is not defined

    ```nextflow
            .combine(SAMTOOLS_FAIDX_CONTIGS.out.fai, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:48:5`: `YAHS` is not defined

    ```nextflow
        YAHS(ch_yahs_input)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:49:35`: `YAHS` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(YAHS.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:54:5`: `SAMTOOLS_FAIDX_SCAFFOLDS` is not defined

    ```nextflow
        SAMTOOLS_FAIDX_SCAFFOLDS(
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:55:9`: `YAHS` is not defined

    ```nextflow
            YAHS.out.scaffolds_fasta,
            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:63:22`: `SAMTOOLS_FAIDX_SCAFFOLDS` is not defined

    ```nextflow
        ch_pairs_input = SAMTOOLS_FAIDX_SCAFFOLDS.out.fai
                         ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:64:18`: `YAHS` is not defined

    ```nextflow
            .combine(YAHS.out.scaffolds_agp, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:65:18`: `SAMTOOLS_FAIDX_CONTIGS` is not defined

    ```nextflow
            .combine(SAMTOOLS_FAIDX_CONTIGS.out.fai, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:66:18`: `YAHS` is not defined

    ```nextflow
            .combine(YAHS.out.binary, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:75:18`: `SAMTOOLS_FAIDX_SCAFFOLDS` is not defined

    ```nextflow
            .combine(SAMTOOLS_FAIDX_SCAFFOLDS.out.sizes, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:92:25`: `YAHS` is not defined

    ```nextflow
        scaffolds_fasta   = YAHS.out.scaffolds_fasta
                            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:93:25`: `YAHS` is not defined

    ```nextflow
        scaffolds_agp     = YAHS.out.scaffolds_agp
                            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:94:25`: `YAHS` is not defined

    ```nextflow
        yahs_bin          = YAHS.out.binary
                            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:95:25`: `YAHS` is not defined

    ```nextflow
        yahs_inital       = YAHS.out.initial_break_agp
                            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:96:25`: `YAHS` is not defined

    ```nextflow
        yahs_intermediate = YAHS.out.round_agp
                            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_bam_scaffolding_yahs/main.nf:97:25`: `YAHS` is not defined

    ```nextflow
        yahs_log          = YAHS.out.log
                            ^^^^^^^^^^
    ```
