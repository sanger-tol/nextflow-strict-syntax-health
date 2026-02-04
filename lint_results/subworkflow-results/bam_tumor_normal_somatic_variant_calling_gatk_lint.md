# Nextflow lint results

- Generated: 2026-02-04T00:20:47.275629+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/nf-core/bam_tumor_normal_somatic_variant_calling_gatk/main.nf:25:16`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      versions = Channel.empty()
                 ^^^^^^^^^^
  ```
