# Nextflow lint results

- Generated: 2026-03-03T00:10:36.673553914Z
- Nextflow version: 26.02.0-edge
- Summary: 6 warnings

## :warning: Warnings

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:33:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      monochrome_logs   // boolean: Do not use coloured log outputs
      ^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_curationpretext_pipeline/main.nf:36:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/sanger-tol/gap_finder/main.nf:45:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          SEQTK_CUTN.out.bed.filter{ meta, file -> val_run_bgzip}
                                     ^^^^
  ```

- Warning: `subworkflows/sanger-tol/gap_finder/main.nf:45:42`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          SEQTK_CUTN.out.bed.filter{ meta, file -> val_run_bgzip}
                                           ^^^^
  ```

- Warning: `subworkflows/sanger-tol/telo_finder/main.nf:132:34`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_telo_bedfiles.filter{ meta, file -> val_run_bgzip}
                                   ^^^^
  ```

- Warning: `subworkflows/sanger-tol/telo_finder/main.nf:132:40`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_telo_bedfiles.filter{ meta, file -> val_run_bgzip}
                                         ^^^^
  ```
