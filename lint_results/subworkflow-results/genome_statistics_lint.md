# Nextflow lint results

- Generated: 2026-08-21T00:08:48.815915+00:00
- Nextflow version: 26.08.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/genome_statistics/main.nf:63:19`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, asms, lineage -> lineage}
                    ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/genome_statistics/main.nf:63:25`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .filter { meta, asms, lineage -> lineage}
                          ^^^^^^^^^^
  ```
