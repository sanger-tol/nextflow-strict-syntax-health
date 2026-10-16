# Nextflow lint results

- Generated: 2026-10-16T00:09:04.700235+00:00
- Nextflow version: 26.10.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/sanger-tol/telomere/findtelomere/main.nf:23:5`: The `when` section is deprecated -- use conditional logic in the calling workflow, or the `process.when` config option to disable a process at runtime

  ```nextflow
      when:
      ^^^^^
  ```
