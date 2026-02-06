# sanger-tol Strict Syntax Health Report

This repository tracks the health of sanger-tol pipelines, modules, and subworkflows with respect to Nextflow's _strict syntax_ linting.

The [Nextflow docs](https://www.nextflow.io/docs/latest/strict-syntax.html) describes the differences from standard Nextflow syntax and includes many examples to help with migration and fixing errors.
Strict syntax is backwards compatible with existing Nextflow code, but enforces stricter rules to catch common errors and improve code quality.

The goal is for all sanger-tol pipelines to run without errors using strict syntax.

> [!IMPORTANT]
> See the [nf-core blog post](https://nf-co.re/blog/2025/nextflow_syntax_nf-core_roadmap) for details on the migration timeline.
> **Fixing all errors from `nextflow lint` will be a requirement by early spring 2026.**

- **Last updated:** 2026-02-06 13:21:41 UTC
- **Nextflow version:** 25.12.0-edge

## Pipelines

- **Total:** 0 parse errors, 205 errors, 641 warnings across 19 pipelines
- **Zero errors:** 9 pipelines (47.4%)

|                    Errors                    |                     Warnings                     |
| :------------------------------------------: | :----------------------------------------------: |
| ![Errors](lint_results/pipelines_errors.png) | ![Warnings](lint_results/pipelines_warnings.png) |

<details>
<summary>Pipeline Results (19 pipelines)</summary>

| Pipeline                                                                                  | Parse Error | Errors | Warnings | Prints Help |                             Lint Output                             |                               Help Output                               |
| ----------------------------------------------------------------------------------------- | :---------: | -----: | -------: | :---------: | :-----------------------------------------------------------------: | :---------------------------------------------------------------------: |
| :x: [genealignment](https://github.com/sanger-tol/genealignment)                          |     No      |     61 |       28 |      -      |     [View](lint_results/pipeline-results/genealignment_lint.md)     |                                    -                                    |
| :x: [blobtoolkit](https://github.com/sanger-tol/blobtoolkit)                              |     No      |     60 |       94 |      -      |      [View](lint_results/pipeline-results/blobtoolkit_lint.md)      |                                    -                                    |
| :x: [genomenote](https://github.com/sanger-tol/genomenote)                                |     No      |     27 |       82 |      -      |      [View](lint_results/pipeline-results/genomenote_lint.md)       |                                    -                                    |
| :x: [treeval](https://github.com/sanger-tol/treeval)                                      |     No      |     21 |      177 |      -      |        [View](lint_results/pipeline-results/treeval_lint.md)        |                                    -                                    |
| :x: [curationpretext](https://github.com/sanger-tol/curationpretext)                      |     No      |     13 |       53 |      -      |    [View](lint_results/pipeline-results/curationpretext_lint.md)    |                                    -                                    |
| :x: [variantcalling](https://github.com/sanger-tol/variantcalling)                        |     No      |     11 |       53 |      -      |    [View](lint_results/pipeline-results/variantcalling_lint.md)     |                                    -                                    |
| :x: [genomeassembly](https://github.com/sanger-tol/genomeassembly)                        |     No      |      5 |       31 |      -      |    [View](lint_results/pipeline-results/genomeassembly_lint.md)     |                                    -                                    |
| :x: [zippypretext](https://github.com/sanger-tol/zippypretext)                            |     No      |      5 |       15 |      -      |     [View](lint_results/pipeline-results/zippypretext_lint.md)      |                                    -                                    |
| :x: [variantcomposition](https://github.com/sanger-tol/variantcomposition)                |     No      |      1 |       17 |      -      |  [View](lint_results/pipeline-results/variantcomposition_lint.md)   |                                    -                                    |
| :x: [ascc](https://github.com/sanger-tol/ascc)                                            |     No      |      1 |        7 |      -      |         [View](lint_results/pipeline-results/ascc_lint.md)          |                                    -                                    |
| :x: [ear](https://github.com/sanger-tol/ear)                                              |     No      |      0 |       52 |     No      |          [View](lint_results/pipeline-results/ear_lint.md)          |          [View](lint_results/prints-help-results/ear_help.txt)          |
| :x: [nfmicrofinder](https://github.com/sanger-tol/nfmicrofinder)                          |     No      |      0 |       21 |     No      |     [View](lint_results/pipeline-results/nfmicrofinder_lint.md)     |     [View](lint_results/prints-help-results/nfmicrofinder_help.txt)     |
| :x: [purging](https://github.com/sanger-tol/purging)                                      |     No      |      0 |        5 |     No      |        [View](lint_results/pipeline-results/purging_lint.md)        |        [View](lint_results/prints-help-results/purging_help.txt)        |
| :x: [readmapping](https://github.com/sanger-tol/readmapping)                              |     No      |      0 |        4 |     No      |      [View](lint_results/pipeline-results/readmapping_lint.md)      |      [View](lint_results/prints-help-results/readmapping_help.txt)      |
| :x: [sequencecomposition](https://github.com/sanger-tol/sequencecomposition)              |     No      |      0 |        2 |     No      |  [View](lint_results/pipeline-results/sequencecomposition_lint.md)  |  [View](lint_results/prints-help-results/sequencecomposition_help.txt)  |
| :x: [ensemblgenedownload](https://github.com/sanger-tol/ensemblgenedownload)              |     No      |      0 |        0 |     No      |  [View](lint_results/pipeline-results/ensemblgenedownload_lint.md)  |  [View](lint_results/prints-help-results/ensemblgenedownload_help.txt)  |
| :x: [ensemblrepeatdownload](https://github.com/sanger-tol/ensemblrepeatdownload)          |     No      |      0 |        0 |     No      | [View](lint_results/pipeline-results/ensemblrepeatdownload_lint.md) | [View](lint_results/prints-help-results/ensemblrepeatdownload_help.txt) |
| :x: [insdcdownload](https://github.com/sanger-tol/insdcdownload)                          |     No      |      0 |        0 |     No      |     [View](lint_results/pipeline-results/insdcdownload_lint.md)     |     [View](lint_results/prints-help-results/insdcdownload_help.txt)     |
| :white_check_mark: [metagenomeassembly](https://github.com/sanger-tol/metagenomeassembly) |     No      |      0 |        0 |     Yes     |  [View](lint_results/pipeline-results/metagenomeassembly_lint.md)   |  [View](lint_results/prints-help-results/metagenomeassembly_help.txt)   |

</details>

## Modules

- **Total:** 0 parse errors, 0 errors, 1 warnings across 20 modules
- **Zero errors:** 20 modules (100.0%)

|                   Errors                   |                    Warnings                    |
| :----------------------------------------: | :--------------------------------------------: |
| ![Errors](lint_results/modules_errors.png) | ![Warnings](lint_results/modules_warnings.png) |

<details>
<summary>Module Results (0 modules with errors)</summary>

| Module | Parse Error | Errors | Warnings | Lint Output |
| ------ | :---------: | -----: | -------: | :---------: |

_Modules with zero errors are not shown above (20 modules). They may still have warnings. See the [modules results directory](lint_results/module-results/) for all lint outputs._

</details>

## Subworkflows

- **Total:** 0 parse errors, 184 errors, 0 warnings across 12 subworkflows
- **Zero errors:** 0 subworkflows (0.0%)

|                     Errors                      |                      Warnings                       |
| :---------------------------------------------: | :-------------------------------------------------: |
| ![Errors](lint_results/subworkflows_errors.png) | ![Warnings](lint_results/subworkflows_warnings.png) |

<details>
<summary>Subworkflow Results (12 subworkflows with errors)</summary>

| Subworkflow                                                                                                                                          | Parse Error | Errors | Warnings |                                   Lint Output                                   |
| ---------------------------------------------------------------------------------------------------------------------------------------------------- | :---------: | -----: | -------: | :-----------------------------------------------------------------------------: |
| :x: [fasta_purge_retained_haplotype](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/fasta_purge_retained_haplotype) |     No      |     43 |        0 | [View](lint_results/subworkflow-results/fasta_purge_retained_haplotype_lint.md) |
| :x: [genome_statistics](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/genome_statistics)                           |     No      |     28 |        0 |       [View](lint_results/subworkflow-results/genome_statistics_lint.md)        |
| :x: [pairs_create_contact_maps](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/pairs_create_contact_maps)           |     No      |     24 |        0 |   [View](lint_results/subworkflow-results/pairs_create_contact_maps_lint.md)    |
| :x: [fasta_bam_scaffolding_yahs](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/fasta_bam_scaffolding_yahs)         |     No      |     20 |        0 |   [View](lint_results/subworkflow-results/fasta_bam_scaffolding_yahs_lint.md)   |
| :x: [cram_map_illumina_hic](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/cram_map_illumina_hic)                   |     No      |     16 |        0 |     [View](lint_results/subworkflow-results/cram_map_illumina_hic_lint.md)      |
| :x: [bam2cool](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/bam2cool)                                             |     No      |     13 |        0 |            [View](lint_results/subworkflow-results/bam2cool_lint.md)            |
| :x: [cram_map_long_reads](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/cram_map_long_reads)                       |     No      |     12 |        0 |      [View](lint_results/subworkflow-results/cram_map_long_reads_lint.md)       |
| :x: [bam_samtools_merge_markdup](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/bam_samtools_merge_markdup)         |     No      |     10 |        0 |   [View](lint_results/subworkflow-results/bam_samtools_merge_markdup_lint.md)   |
| :x: [gap_finder](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/gap_finder)                                         |     No      |      7 |        0 |           [View](lint_results/subworkflow-results/gap_finder_lint.md)           |
| :x: [fastx_map_long_reads](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/fastx_map_long_reads)                     |     No      |      4 |        0 |      [View](lint_results/subworkflow-results/fastx_map_long_reads_lint.md)      |
| :x: [telo_finder](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/telo_finder)                                       |     No      |      4 |        0 |          [View](lint_results/subworkflow-results/telo_finder_lint.md)           |
| :x: [ancestral_annotation](https://github.com/sanger-tol/nf-core-modules/tree/main/subworkflows/sanger-tol/ancestral_annotation)                     |     No      |      3 |        0 |      [View](lint_results/subworkflow-results/ancestral_annotation_lint.md)      |

</details>

## About

This report is generated daily by running `nextflow lint` on each sanger-tol pipeline, module, and subworkflow.
The linting checks for strict syntax compliance in Nextflow DSL2 code.

- **Parse errors** indicate items where `nextflow lint` could not run at all, typically due to syntax errors that prevent Nextflow from parsing the code
- **Errors** indicate syntax issues that will cause problems in future Nextflow versions
- **Warnings** indicate deprecated patterns that should be updated, but having warnings is fine (though it's nice to fix those as well if possible)
- **Prints Help** (pipelines only) tests whether the pipeline can print its help message using the v2 syntax parser (`NXF_SYNTAX_PARSER=v2 nextflow run . --help`). This test only runs for pipelines with zero lint errors.

## Running Locally

You can run `nextflow lint` on your own pipeline to check for strict syntax issues:

```bash
nextflow lint .
```

> **Note:** Until [this fix](https://github.com/nextflow-io/nextflow/pull/6716) is included in a Nextflow edge release, you may need to exclude nf-test files manually:
>
> ```bash
> nextflow lint . -exclude ".git,.nf-test,nf-test.config"
> ```

See the [strict syntax documentation](https://www.nextflow.io/docs/latest/strict-syntax.html) for more information about the rules being checked.

## Getting Help

If you need help fixing strict syntax errors in your pipeline, the [Nextflow community forum](https://community.seqera.io/) is a great place to ask questions.
