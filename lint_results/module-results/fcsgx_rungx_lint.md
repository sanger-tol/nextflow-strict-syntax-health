# Nextflow lint results

- Generated: 2026-10-25T00:06:34.540734+00:00
- Nextflow version: 26.10.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/fcsgx/rungx/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
