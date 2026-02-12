# Nextflow lint results

- Generated: 2026-02-12T00:09:50.997658+00:00
- Nextflow version: 26.01.1-edge
- Summary: 10 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:22:5`: Variable was declared but not used

  ```nextflow
      untrimmed_cram = channel.empty()
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:23:5`: Variable was declared but not used

  ```nextflow
      untrimmed_fastx = channel.empty()
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:25:5`: Variable was declared but not used

  ```nextflow
      trimmed_cram = channel.empty()
      ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:63:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      hifitrimmer_summary = Channel.empty()
                            ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:64:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      hifitrimmer_bed = Channel.empty()
                        ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:69:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, reads, yaml -> !yaml }
                        ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:69:29`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .filter { meta, reads, yaml -> !yaml }
                              ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:70:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, reads, yaml -> [meta, reads] }
                                  ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:74:26`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .subscribe { meta, reads ->
                           ^^^^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:82:33`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .map { meta, reads, yaml -> [meta, reads] }
                                  ^^^^^^^^^^
  ```
