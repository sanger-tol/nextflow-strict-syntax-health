# Nextflow lint results

- Generated: 2026-05-27T00:27:33.515188+00:00
- Nextflow version: 26.04.2
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/busco_gene/main.nf:62:81`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gz_index               = val_zip_bedgraph ? TABIX_BGZIPTABIX.out.gz_index : Channel.empty()
                                                                                  ^^^^^^^^^^
  ```
