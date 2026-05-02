# Nextflow lint results

- Generated: 2026-05-02T00:19:16.722393409Z
- Nextflow version: 26.04.0
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/binning/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      ch_contig2bin = channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:37:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      val_rrna_prediction // boolean: enable rrna prediction
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:135:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  BINNING.out.contig2bin.filter { meta, c2b -> meta.binner != "circular" },
                                                        ^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:241:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
