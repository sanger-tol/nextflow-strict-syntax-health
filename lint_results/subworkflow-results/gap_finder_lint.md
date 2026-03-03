# Nextflow lint results

- Generated: 2026-03-03T00:11:06.871457+00:00
- Nextflow version: 26.02.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/gap_finder/main.nf:45:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          SEQTK_CUTN.out.bed.filter{ meta, file -> val_run_bgzip}
                                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/gap_finder/main.nf:45:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          SEQTK_CUTN.out.bed.filter{ meta, file -> val_run_bgzip}
                                           ^^^^^^^^^^
  ```
