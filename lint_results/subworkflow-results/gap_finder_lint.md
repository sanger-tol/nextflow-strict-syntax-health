# Nextflow lint results

- Generated: 2026-02-28T00:08:35.397363+00:00
- Nextflow version: 26.01.1-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/gap_finder/main.nf:38:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          SEQTK_CUTN.out.bed.filter{ meta, file -> val_run_bgzip}
                                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/gap_finder/main.nf:38:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          SEQTK_CUTN.out.bed.filter{ meta, file -> val_run_bgzip}
                                           ^^^^^^^^^^
  ```
