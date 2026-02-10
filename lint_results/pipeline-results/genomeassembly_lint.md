# Nextflow lint results

- Generated: 2026-02-10T00:12:05.405641796Z
- Nextflow version: 26.01.0-edge
- Summary: 25 warnings

## :warning: Warnings

- Warning: `modules/nf-core/bcftools/consensus/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/bcftools/consensus/main.nf:42:9`: Variable was declared but not used

  ```nextflow
      def masking = mask ? "-m $mask" : ""
          ^^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:23:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/bcftools/index/main.nf:40:9`: Variable was declared but not used

  ```nextflow
      def prefix = task.ext.prefix ?: "${meta.id}"
          ^^^^^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:23:40`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list = files_in.collect { it.toString() }
                                         ^^
  ```

- Warning: `modules/nf-core/cat/cat/main.nf:58:42`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def file_list   = files_in.collect { it.toString() }
                                           ^^
  ```

- Warning: `modules/nf-core/gatk4/mergevcfs/main.nf:25:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_list = vcf.collect{ "--INPUT $it"}.join(' ')
                                             ^^
  ```

- Warning: `modules/nf-core/genomescope2/main.nf:47:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:30:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_mat       = matktab   ? "${matktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}"   : ''
                                                     ^^
  ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:31:52`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_pat       = patktab   ? "${patktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}"   : ''
                                                     ^^
  ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:32:54`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def input_child = childktab ? "${childktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}" : ''
                                                       ^^
  ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:43:9`: Variable was declared but not used

  ```nextflow
      def args  = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:44:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_mat = matktab ? "${matktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}" : ''
                                             ^^
  ```

- Warning: `modules/nf-core/merquryfk/hapmaker/main.nf:45:44`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      input_pat = patktab ? "${patktab.find{ it.toString().endsWith(".ktab") }.toString() - ~/\.ktab/}" : ''
                                             ^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:39:56`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def fk_ktab     = fastk_ktab ? "${fastk_ktab.find{ it.toString().endsWith(".ktab") }}" : ''
                                                         ^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:40:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def mat_hapktab = mathaptab  ? "${mathaptab.find{ it.toString().endsWith(".ktab") }}"  : ''
                                                        ^^
  ```

- Warning: `modules/nf-core/merquryfk/merquryfk/main.nf:41:55`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def pat_hapktab = pathaptab  ? "${pathaptab.find{ it.toString().endsWith(".ktab") }}"  : ''
                                                        ^^
  ```

- Warning: `modules/nf-core/minimap2/align/main.nf:67:9`: Variable was declared but not used

  ```nextflow
      def target = reference ?: (bam_input ? error("BAM input requires reference") : reads)
          ^^^^^^
  ```

- Warning: `modules/nf-core/seqkit/grep/main.nf:46:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `modules/sanger-tol/samtools/mergedup/main.nf:56:9`: Variable was declared but not used

  ```nextflow
      def args      = task.ext.args  ?: ''
          ^^^^
  ```

- Warning: `modules/sanger-tol/yak/count/main.nf:36:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/nf-core/bam_stats_samtools/main.nf:15:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:25:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/genomeassembly.nf:73:26`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      def topic_versions = Channel.topic("versions")
                           ^^^^^^^
  ```

- Warning: `workflows/genomeassembly.nf:97:17`: Variable was declared but not used

  ```nextflow
          ).set { ch_collated_versions }
                  ^^^^^^^^^^^^^^^^^^^^
  ```
