# Nextflow lint results

- Generated: 2026-05-20T00:27:43.427620156Z
- Nextflow version: 26.04.1
- Summary: 1 error, 10 warnings

## :x: Errors

- Error: `subworkflows/local/utils_nfcore_busco_pipeline/main.nf:110:20`: `fasta` is already declared

    ```nextflow
                .map { fasta -> [fasta, null, null] }
                       ^^^^^
    ```


## :warning: Warnings

- Warning: `main.nf:42:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        multiqc_report = BUSCO.out.multiqc_report // channel: /path/to/multiqc_report.html
        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_busco_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs   // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:43:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        dummy_emit = true
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

    ```nextflow
        valid_config = checkConfigProvided()
        ^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:20:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        valid_config
        ^^^^^^^^^^^^
    ```

- Warning: `subworkflows/nf-core/utils_nfschema_plugin/main.nf:72:5`: Emit name should be omitted when there is only one emit

    ```nextflow
        dummy_emit = true
        ^^^^^^^^^^^^^^^
    ```

- Warning: `workflows/busco.nf:35:19`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .branch { meta, fasta ->
                      ^^^^
    ```

- Warning: `workflows/busco.nf:59:31`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            ch_genome.map { meta, fasta -> meta.lineage },
                                  ^^^^^
    ```

- Warning: `workflows/busco.nf:71:41`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .combine( ch_genome.map { meta, fasta -> meta.lineage } )
                                            ^^^^^
    ```

- Warning: `workflows/busco.nf:88:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        def topic_versions = Channel.topic("versions")
                             ^^^^^^^
    ```
