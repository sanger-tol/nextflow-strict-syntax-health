# Nextflow lint results

- Generated: 2026-02-06T13:21:14.637771004Z
- Nextflow version: 25.12.0-edge
- Summary: 1 error, 17 warnings

## :x: Errors

- Error: `conf/modules.config:25:9`: If statements cannot be mixed with config statements

    ```nextflow
            if (params.include_positions) {
            ^
    ```


## :warning: Warnings

- Warning: `modules/nf-core/pigz/compress/main.nf:35:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/tar/main.nf:65:9`: Variable was declared but not used

    ```nextflow
        def args = task.ext.args ?: ''
            ^^^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:97:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--bed') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:98:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--exclude-bed') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:99:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--hapcount') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:100:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--positions') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:101:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--exclude-positions') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:106:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--diff') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:107:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--gzdiff') }
                             ^^
    ```

- Warning: `modules/nf-core/vcftools/main.nf:108:26`: Implicit closure parameter is deprecated, declare an explicit parameter instead

    ```nextflow
        args_list.removeIf { it.contains('--diff-bcf') }
                             ^^
    ```

- Warning: `subworkflows/local/bcftools_stats_plot/main.nf:11:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/features/main.nf:17:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        ch_versions = Channel.empty()
                      ^^^^^^^
    ```

- Warning: `subworkflows/local/features/main.nf:21:25`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
            .branch { meta, data ->
                            ^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcomposition_pipeline/main.nf:32:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        monochrome_logs   // boolean: Do not use coloured log outputs
        ^^^^^^^^^^^^^^^
    ```

- Warning: `subworkflows/local/utils_nfcore_variantcomposition_pipeline/main.nf:35:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        input             //  string: Path to input samplesheet
        ^^^^^
    ```

- Warning: `workflows/variantcomposition.nf:69:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

    ```nextflow
        def topic_versions = Channel.topic("versions")
                             ^^^^^^^
    ```

- Warning: `workflows/variantcomposition.nf:93:17`: Variable was declared but not used

    ```nextflow
            ).set { ch_collated_versions }
                    ^^^^^^^^^^^^^^^^^^^^
    ```
