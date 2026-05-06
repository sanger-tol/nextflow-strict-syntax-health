# Nextflow lint results

- Generated: 2026-05-06T00:21:12.585995363Z
- Nextflow version: 26.04.0
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/binning/main.nf:31:5`: Variable was declared but not used

  ```nextflow
      ch_contig2bin = channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      val_rrna_prediction // boolean: enable rrna prediction
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:140:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  BINNING.out.contig2bin.filter { meta, c2b -> meta.binner != "circular" },
                                                        ^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:246:9`: Variable was declared but not used

  ```nextflow
      def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
          ^^^^^^^^^^^^^^^^^^^^
  ```
