# Nextflow lint results

- Generated: 2026-02-04T00:20:34.629341+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `modules/nf-core/jvarkit/sam2tsv/main.nf:24:9`: `regions_file` is already declared

  ```nextflow
      def regions_file = regions_file ? " --regions" + " '${regions_file}' " : ""
          ^^^^^^^^^^
  ```
