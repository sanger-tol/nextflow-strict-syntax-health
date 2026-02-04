# Nextflow lint results

- Generated: 2026-02-04T00:20:34.644896+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `modules/nf-core/merquryfk/katgc/main.nf:31:28`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          ${fastk_ktab.find{ it.toString().endsWith(".ktab") }} \\
                             ^^^^^^^^^^
  ```
