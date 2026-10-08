# Nextflow lint results

- Generated: 2026-10-08T15:37:03.396503371Z
- Nextflow version: 26.09.2-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `workflows/tollongc.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_samplesheet // channel: samplesheet read in from --input
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/tollongc.nf:46:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
