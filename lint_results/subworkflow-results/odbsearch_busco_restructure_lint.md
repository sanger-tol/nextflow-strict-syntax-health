# Nextflow lint results

- Generated: 2026-07-03T00:26:11.137116+00:00
- Nextflow version: 26.06.0-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:40:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, odb, ref_meta, ref -> [ ref_meta, odb, ref ] }  // meta == ref_meta thanks to APISCRIPTS_GETLINEAGEODBS
                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:40:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, odb, ref_meta, ref -> [ ref_meta, odb, ref ] }  // meta == ref_meta thanks to APISCRIPTS_GETLINEAGEODBS
                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:41:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .unique { meta, odb, ref ->
                               ^^^^^^
  ```
