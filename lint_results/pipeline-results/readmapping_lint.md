# Nextflow lint results

- Generated: 2026-09-19T00:07:49.904331594Z
- Nextflow version: 26.08.0-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `subworkflows/local/align_long.nf:147:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [ meta + [ read_group: rg_args, add_rg: !rglines.any { it.contains('SM:') } ], bam ]
                                                                     ^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:70:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          ch_hifitrimmer_branch = ch_hifitrimmer_input.branch { meta, reads ->
                                                                      ^^^^^
  ```

- Warning: `subworkflows/sanger-tol/pacbio_preprocess/main.nf:99:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
              .join(ch_hifitrimmer_branch.trim.map { meta, reads -> [ meta - meta.subMap('_adapter_yaml'), meta._adapter_yaml ] }, by: 0)
                                                           ^^^^^
  ```

- Warning: `workflows/readmapping.nf:52:5`: Variable was declared but not used

  ```nextflow
      multiqc_report   = channel.empty()
      ^^^^^^^^^^^^^^
  ```
