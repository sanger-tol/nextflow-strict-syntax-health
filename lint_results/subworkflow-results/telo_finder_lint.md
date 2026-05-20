# Nextflow lint results

- Generated: 2026-05-20T00:27:57.566378+00:00
- Nextflow version: 26.04.1
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/telo_finder/main.nf:54:70`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      gz_index         = val_zip_bed ? TABIX_BGZIPTABIX.out.gz_index : Channel.empty()
                                                                       ^^^^^^^^^^
  ```
