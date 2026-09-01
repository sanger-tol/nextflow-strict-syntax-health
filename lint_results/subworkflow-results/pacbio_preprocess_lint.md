# Nextflow lint results

- Generated: 2026-09-01T00:12:27.457455+00:00
- Nextflow version: 26.08.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:70:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_hifitrimmer_branch = ch_hifitrimmer_input.branch { meta, reads ->
                                                                      ^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:99:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .join(ch_hifitrimmer_branch.trim.map { meta, reads -> [ meta - meta.subMap('_adapter_yaml'), meta._adapter_yaml ] }, by: 0)
                                                           ^^^^^^^^^^
  ```
