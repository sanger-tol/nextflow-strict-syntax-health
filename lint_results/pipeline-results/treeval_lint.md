# Nextflow lint results

- Generated: 2026-04-16T23:49:05.836416358Z
- Nextflow version: 26.03.2-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/local/selfcomp/splitfasta/main.nf:25:9`: Variable was declared but not used

  ```nextflow
      def VERSION     = "1.7.8-1"
          ^^^^^^^
  ```

- Warning: `modules/local/selfcomp/splitfasta/main.nf:32:9`: Variable was declared but not used

  ```nextflow
      def VERSION     = "1.7.8-1"
          ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```
