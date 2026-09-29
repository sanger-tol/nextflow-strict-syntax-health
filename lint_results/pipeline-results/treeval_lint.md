# Nextflow lint results

- Generated: 2026-09-29T00:09:39.645064958Z
- Nextflow version: 26.09.1-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/nf-core/fasta_clean_faidx/main.nf:91:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          renamed_fasta.filter { meta, file -> val_get_dict }
                                 ^^^^
  ```

- Warning: `subworkflows/nf-core/fasta_clean_faidx/main.nf:91:38`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          renamed_fasta.filter { meta, file -> val_get_dict }
                                       ^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:98`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      return ch_versions.unique().map { version -> processVersionsFromYAML(version) }.unique().mix(Channel.of(workflowVersionToYAML()))
                                                                                                   ^^^^^^^
  ```

- Warning: `workflows/treeval.nf:54:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      map_order       // channel: hic mapping order (from yaml)
      ^^^^^^^^^
  ```
