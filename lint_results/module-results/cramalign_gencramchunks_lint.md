# Nextflow lint results

- Generated: 2026-10-23T00:10:21.470234+00:00
- Nextflow version: 26.10.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/cramalign/gencramchunks/main.nf:14:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
