# Nextflow lint results

- Generated: 2026-09-02T00:08:34.581449863Z
- Nextflow version: 26.08.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             // string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `workflows/curationpretext.nf:301:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
