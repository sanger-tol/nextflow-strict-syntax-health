# Nextflow lint results

- Generated: 2026-10-08T15:36:37.841866348Z
- Nextflow version: 26.09.2-edge
- Summary: 3 warnings

## :warning: Warnings

- Warning: `modules/nf-core/samtools/merge/main.nf:57:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/align_long.nf:152:68`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [ meta + [ read_group: rg_args, add_rg: !rglines.any { it.contains('SM:') } ], bam ]
                                                                     ^^
  ```

- Warning: `workflows/readmapping.nf:54:5`: Variable was declared but not used

  ```nextflow
      multiqc_report   = channel.empty()
      ^^^^^^^^^^^^^^
  ```
