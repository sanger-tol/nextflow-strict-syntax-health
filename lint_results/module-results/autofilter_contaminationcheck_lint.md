# Nextflow lint results

- Generated: 2026-07-25T00:24:07.580884+00:00
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/autofilter/contaminationcheck/main.nf:26:9`: Variable was declared but not used

    ```nextflow
        def args    = task.ext.args     ?: ""
            ^^^^^^^^^^
    ```
