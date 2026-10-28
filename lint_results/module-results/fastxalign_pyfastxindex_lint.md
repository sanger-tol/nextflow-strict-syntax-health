# Nextflow lint results

- Generated: 2026-10-28T00:08:14.037570+00:00
- Nextflow version: 26.10.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/fastxalign/pyfastxindex/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
