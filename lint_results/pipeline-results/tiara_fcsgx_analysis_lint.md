# Nextflow lint results

- Generated: 2026-10-29T00:06:59.382256420Z
- Nextflow version: 26.10.3
- Summary: 2 warnings

## :warning: Warnings

- Warning: `workflows/tiara_fcsgx_analysis.nf:19:5`: Parameter was not used -- prefix with `_` to suppress warning

    ```nextflow
        ch_samplesheet // channel: samplesheet read in from --input
        ^^^^^^^^^^^^^^
    ```

- Warning: `workflows/tiara_fcsgx_analysis.nf:46:9`: Variable was declared but not used

    ```nextflow
        def ch_collated_versions = softwareVersionsToYAML(ch_versions.mix(topic_versions.versions_file))
            ^^^^^^^^^^^^^^^^^^^^
    ```
