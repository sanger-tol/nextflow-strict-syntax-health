# Nextflow lint results

- Generated: 2026-08-20T00:08:04.421864966Z
- Nextflow version: 26.07.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `workflows/nfmicrofinder.nf:68:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
