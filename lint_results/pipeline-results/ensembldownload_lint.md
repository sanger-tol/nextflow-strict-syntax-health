# Nextflow lint results

- Generated: 2026-11-18T00:05:39.598697713Z
- Nextflow version: 26.11.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `workflows/ensembldownload.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_samplesheet // channel: samplesheet read in from --input
      ^^^^^^^^^^^^^^
  ```

- Warning: `workflows/ensembldownload.nf:46:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
