# Nextflow lint results

- Generated: 2026-10-08T15:37:51.475147863Z
- Nextflow version: 26.09.2-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `subworkflows/local/af_roh/main.nf:58:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_vcf:  it[1] == null
                       ^^
  ```

- Warning: `subworkflows/local/af_roh/main.nf:59:22`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              no_af:   it[4] == null
                       ^^
  ```

- Warning: `subworkflows/local/af_roh/main.nf:64:36`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch.no_vcf.map { id, _null, af, af_tbi ->
                                     ^^^^^^
  ```
