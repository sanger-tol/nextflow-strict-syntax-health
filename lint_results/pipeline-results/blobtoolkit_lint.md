# Nextflow lint results

- Generated: 2026-05-13T00:23:01.766792074Z
- Nextflow version: 26.04.1
- Summary: 4 warnings

## :warning: Warnings

- Warning: `conf/modules.config:136:23`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              saveAs: { filename ->
                        ^^^^^^^^
  ```

- Warning: `subworkflows/local/busco_diamond_blastp.nf:232:5`: Variable was declared but not used

  ```nextflow
      multiqc = BUSCO_BUSCO.out.short_summaries_txt
      ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:16:5`: Variable was declared but not used

  ```nextflow
      valid_config = checkConfigProvided()
      ^^^^^^^^^^^^
  ```

- Warning: `workflows/blobtoolkit.nf:178:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```
