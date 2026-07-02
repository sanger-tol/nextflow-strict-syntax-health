# Nextflow lint results

- Generated: 2026-07-02T00:29:16.533982+00:00
- Nextflow version: 26.06.0-edge
- Summary: 5 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:23:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_taxid.map{ meta, taxid -> taxid },
                        ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:24:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_specified_lineages.map{ meta, taxid -> taxid }
                                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:44:16`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, odb, ref_meta, ref -> [ ref_meta, odb, ref ] }  // meta == ref_meta thanks to APISCRIPTS_GETLINEAGEODBS
                 ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:44:20`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { id, meta, odb, ref_meta, ref -> [ ref_meta, odb, ref ] }  // meta == ref_meta thanks to APISCRIPTS_GETLINEAGEODBS
                     ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/odbsearch_busco_restructure/main.nf:45:30`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .unique { meta, odb, ref ->
                               ^^^^^^
  ```
