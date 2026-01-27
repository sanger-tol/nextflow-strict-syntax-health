# Nextflow lint results

- Generated: 2026-01-27T00:18:46.853931+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/sourmash/compare/main.nf:32:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def sigs = signatures ? "${signatures.sort{it.toString()}.join(' ')}" : ''
                                                 ^^^^^^^^^^
  ```
