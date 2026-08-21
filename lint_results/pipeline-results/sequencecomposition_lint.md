# Nextflow lint results

- Generated: 2026-08-21T00:08:29.707541288Z
- Nextflow version: 26.08.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `workflows/sequencecomposition.nf:74:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
