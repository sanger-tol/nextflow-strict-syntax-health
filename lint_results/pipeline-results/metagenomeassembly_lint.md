# Nextflow lint results

- Generated: 2026-04-30T00:22:08.744218187Z
- Nextflow version: 26.04.0
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/binning/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      ch_contig2bin = channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:37:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      val_rrna_prediction // boolean: enable rrna prediction
      ^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `workflows/metagenomeassembly.nf:134:55`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  BINNING.out.contig2bin.filter { meta, c2b -> meta.binner != "circular" },
                                                        ^^^
  ```
