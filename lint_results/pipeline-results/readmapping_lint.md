# Nextflow lint results

- Generated: 2026-07-30T00:21:52.380428832Z
- Nextflow version: 26.07.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/align_long.nf:87:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
                  .branch { meta, yaml ->
                                  ^^^^
  ```

- Warning: `subworkflows/local/align_short.nf:39:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .branch { meta, cram ->
                          ^^^^
  ```
