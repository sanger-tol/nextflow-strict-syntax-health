# Nextflow lint results

- Generated: 2026-03-03T00:11:06.872113+00:00
- Nextflow version: 26.02.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/telo_finder/main.nf:132:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_telo_bedfiles.filter{ meta, file -> val_run_bgzip}
                                   ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/telo_finder/main.nf:132:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_telo_bedfiles.filter{ meta, file -> val_run_bgzip}
                                         ^^^^^^^^^^
  ```
