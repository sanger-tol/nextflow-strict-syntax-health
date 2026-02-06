# sanger-tol Strict Syntax Health Report

This repository tracks the health of sanger-tol pipelines, modules, and subworkflows with respect to Nextflow's _strict syntax_ linting.

The [Nextflow docs](https://www.nextflow.io/docs/latest/strict-syntax.html) describes the differences from standard Nextflow syntax and includes many examples to help with migration and fixing errors.
Strict syntax is backwards compatible with existing Nextflow code, but enforces stricter rules to catch common errors and improve code quality.

The goal is for all sanger-tol pipelines to run without errors using strict syntax.

> [!IMPORTANT]
> See the [nf-core blog post](https://nf-co.re/blog/2025/nextflow_syntax_nf-core_roadmap) for details on the migration timeline.
> **Fixing all errors from `nextflow lint` will be a requirement by early spring 2026.**

- **Last updated:** 2026-02-06 15:11:08 UTC
- **Nextflow version:** 25.12.0-edge

## Subworkflows

- **Total:** 0 parse errors, 0 errors, 0 warnings across 12 subworkflows
- **Zero errors:** 12 subworkflows (100.0%)

|                     Errors                      |                      Warnings                       |
| :---------------------------------------------: | :-------------------------------------------------: |
| ![Errors](lint_results/subworkflows_errors.png) | ![Warnings](lint_results/subworkflows_warnings.png) |

<details>
<summary>Subworkflow Results (0 subworkflows with errors)</summary>

| Subworkflow | Parse Error | Errors | Warnings | Lint Output |
| ----------- | :---------: | -----: | -------: | :---------: |

_Subworkflows with zero errors are not shown above (12 subworkflows). They may still have warnings. See the [subworkflows results directory](lint_results/subworkflow-results/) for all lint outputs._

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
