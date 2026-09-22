# Nextflow lint results

- Generated: 2026-09-22T00:08:32.970046036Z
- Nextflow version: 26.08.0-edge
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

- Warning: `subworkflows/local/yaml_input/main.nf:17:17`: Variable was declared but not used

  ```nextflow
              def kmer_len = data?.kmer_profile?.kmer_length // Will return null if not exist
                  ^^^^^^^^
  ```
