# Nextflow lint results

- Generated: 2026-06-19T00:37:35.463369+00:00
- Nextflow version: 26.04.3
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/sanger-tol/zippypretext/main.nf:32:35`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            ch_zippy_inputs.agp.map { meta, agp -> agp }
                                      ^^^^^^^^^^
    ```

- Warning: `subworkflows/sanger-tol/zippypretext/main.nf:37:52`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            PRETEXT_PRETEXT2ASM.out.correctedagp.map { meta, agp -> agp },
                                                       ^^^^^^^^^^
    ```

- Warning: `subworkflows/sanger-tol/zippypretext/main.nf:38:39`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            ch_zippy_inputs.idxfile.map { meta, idx -> idx }
                                          ^^^^^^^^^^
    ```
