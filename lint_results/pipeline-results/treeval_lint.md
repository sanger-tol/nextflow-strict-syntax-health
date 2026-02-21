# Nextflow lint results

- Generated: 2026-02-21T00:08:11.463783434Z
- Nextflow version: 26.01.1-edge
- Summary: 1 warning

## :warning: Warnings

- Warning: `subworkflows/local/generate_sorted_genome/main.nf:31:23`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .view{"SIZES: $it"}
                        ^^
  ```
