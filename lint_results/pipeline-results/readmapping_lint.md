# Nextflow lint results

- Generated: 2026-02-08T00:13:35.425316760Z
- Nextflow version: 25.12.0-edge
- Summary: 4 warnings

## :warning: Warnings

- Warning: `modules/nf-core/blast/blastn/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:62:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/pigz/compress/main.nf:30:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/tar/main.nf:65:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```
