# Nextflow lint results

- Generated: 2026-05-04T00:18:32.149057+00:00
- Nextflow version: 26.04.0
- Summary: 1 error

## :x: Errors

- Error: `subworkflows/sanger-tol/fasta_compress_index/main.nf:17:27`: Incorrect number of call arguments, expected 2 but received 1

  ```nextflow
      ch_compressed_fasta = SAMTOOLS_BGZIP(ch_fasta).fasta
                            ^^^^^^^^^^
  ```
