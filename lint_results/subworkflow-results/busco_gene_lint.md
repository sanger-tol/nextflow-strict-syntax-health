# Nextflow lint results

- Generated: 2026-06-19T00:37:35.461404+00:00
- Nextflow version: 26.04.3
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/busco_gene/main.nf:58:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, gz, _meta2, idx -> idx.name.startsWith(gz.name) }
                        ^^^^^^^^^^
  ```
