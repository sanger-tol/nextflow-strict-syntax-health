# Nextflow lint results

- Generated: 2026-10-16T00:09:04.699372+00:00
- Nextflow version: 26.10.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/pretext/pretext2asm/main.nf:17:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
