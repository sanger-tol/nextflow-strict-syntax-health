# Nextflow lint results

- Generated: 2026-02-04T00:20:34.607042+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/gatk4/mergevcfs/main.nf:25:47`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = vcf.collect { "--INPUT ${it}" }.join(' ')
                                                ^^^^^^^^^^
  ```
