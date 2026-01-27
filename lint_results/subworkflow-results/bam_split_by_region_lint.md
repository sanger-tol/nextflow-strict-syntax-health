# Nextflow lint results

- Generated: 2026-01-27T00:18:59.467991+00:00
- Nextflow version: 25.12.0-edge
- Summary: 1 error

## :x: Errors

- Error: `subworkflows/nf-core/bam_split_by_region/main.nf:29:44`: Unexpected input: '='

  ```nextflow
              if (! stats['start'] ) [ chrom = stats['seq_name'] ]
                                             ^^^^^^^^^^
  ```
