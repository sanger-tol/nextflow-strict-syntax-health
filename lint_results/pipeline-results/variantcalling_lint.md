# Nextflow lint results

- Generated: 2026-09-12T00:08:33.129658581Z
- Nextflow version: 26.08.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/input_filter_split.nf:19:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_fasta_for_split = fasta.map { meta, fa, fai -> [meta, fa] }
                                                 ^^^
  ```

- Warning: `workflows/variantcalling.nf:55:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      }.branch { meta, fa ->
                 ^^^^
  ```
