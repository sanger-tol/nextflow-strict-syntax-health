# Nextflow lint results

- Generated: 2026-10-09T00:09:25.912048+00:00
- Nextflow version: 26.09.2-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/autofilter/contaminationcheck/main.nf:21:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
