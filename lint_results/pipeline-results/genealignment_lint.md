# Nextflow lint results

- Generated: 2026-02-06T13:19:08.630361785Z
- Nextflow version: 25.12.0-edge
- Summary: 61 errors, 28 warnings

## :x: Errors

- Error: `conf/base.config:14:16`: `check_max` is not defined

  ```nextflow
      cpus   = { check_max( 1    * task.attempt, 'cpus'   ) }
                 ^^^^^^^^^
  ```

- Error: `conf/base.config:15:16`: `check_max` is not defined

  ```nextflow
      memory = { check_max( 6.GB * task.attempt, 'memory' ) }
                 ^^^^^^^^^
  ```

- Error: `conf/base.config:16:16`: `check_max` is not defined

  ```nextflow
      time   = { check_max( 4.h  * task.attempt, 'time'   ) }
                 ^^^^^^^^^
  ```

- Error: `conf/base.config:30:20`: `check_max` is not defined

  ```nextflow
          cpus   = { check_max( 1                  , 'cpus'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:31:20`: `check_max` is not defined

  ```nextflow
          memory = { check_max( 6.GB * task.attempt, 'memory'  ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:32:20`: `check_max` is not defined

  ```nextflow
          time   = { check_max( 4.h  * task.attempt, 'time'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:35:20`: `check_max` is not defined

  ```nextflow
          cpus   = { check_max( 2     * task.attempt, 'cpus'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:36:20`: `check_max` is not defined

  ```nextflow
          memory = { check_max( 12.GB * task.attempt, 'memory'  ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:37:20`: `check_max` is not defined

  ```nextflow
          time   = { check_max( 4.h   * task.attempt, 'time'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:40:20`: `check_max` is not defined

  ```nextflow
          cpus   = { check_max( 6     * task.attempt, 'cpus'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:41:20`: `check_max` is not defined

  ```nextflow
          memory = { check_max( 36.GB * task.attempt, 'memory'  ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:42:20`: `check_max` is not defined

  ```nextflow
          time   = { check_max( 8.h   * task.attempt, 'time'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:45:20`: `check_max` is not defined

  ```nextflow
          cpus   = { check_max( 12    * task.attempt, 'cpus'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:46:20`: `check_max` is not defined

  ```nextflow
          memory = { check_max( 72.GB * task.attempt, 'memory'  ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:47:20`: `check_max` is not defined

  ```nextflow
          time   = { check_max( 16.h  * task.attempt, 'time'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:50:20`: `check_max` is not defined

  ```nextflow
          time   = { check_max( 20.h  * task.attempt, 'time'    ) }
                     ^^^^^^^^^
  ```

- Error: `conf/base.config:53:20`: `check_max` is not defined

  ```nextflow
          memory = { check_max( 200.GB * task.attempt, 'memory' ) }
                     ^^^^^^^^^
  ```

- Error: `modules/nf-core/custom/getchromsizes/main.nf:40:9`: `suffix` is already declared

  ```nextflow
      def suffix  = 'temp.genome'
          ^^^^^^
  ```

- Error: `modules/nf-core/multiqc/main.nf:28:31`: Unexpected input: '/'

  ```nextflow
      def logo = multiqc_logo ? /--cl-config 'custom_logo: "${multiqc_logo}"'/ : ''
                                ^
  ```

- Error: `nextflow.config:59:5`: Unexpected input: 'includeConfig'

  ```nextflow
      includeConfig "${params.custom_config_base}/nfcore_custom.config"
      ^
  ```

- Error: `subworkflows/local/gene_alignment.nf:59:19`: Unexpected input: '->'

  ```nextflow
          .map( row ->
                    ^
  ```

- Error: `subworkflows/local/pep_alignments.nf:3:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import java.math.RoundingMode;
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/pep_alignments.nf:4:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import java.math.BigDecimal;
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_genealignment_pipeline/main.nf:14:1`: Module could not be parsed: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/pipelines/genealignment/subworkflows/nf-core/utils_nextflow_pipeline/main.nf'

  ```nextflow
  include { UTILS_NEXTFLOW_PIPELINE   } from '../../nf-core/utils_nextflow_pipeline'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/local/utils_nfcore_genealignment_pipeline/main.nf:47:5`: `UTILS_NEXTFLOW_PIPELINE` is not defined

  ```nextflow
      UTILS_NEXTFLOW_PIPELINE (
      ^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nextflow_pipeline/main.nf:111:14`: Unexpected input: 'i'

  ```nextflow
      for (int i = 0; i < n - 1; i++) {
               ^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:5:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import org.yaml.snakeyaml.Yaml
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:6:1`: Groovy `import` declarations are not supported -- use fully-qualified name inline instead

  ```nextflow
  import nextflow.extension.FilesEx
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:37:5`: `valid_config` was assigned but not declared

  ```nextflow
      valid_config = true
      ^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:45:9`: `valid_config` was assigned but not declared

  ```nextflow
          valid_config = false
          ^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:47:12`: `valid_config` is not defined

  ```nextflow
      return valid_config
             ^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:99:17`: `Yaml` is not defined

  ```nextflow
      Yaml yaml = new Yaml()
                  ^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:100:5`: `versions` was assigned but not declared

  ```nextflow
      versions = yaml.load(yaml_file).collectEntries { k, v -> [ k.tokenize(':')[-1], v ] }
      ^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:101:27`: `versions` is not defined

  ```nextflow
      return yaml.dumpAsMap(versions).trim()
                            ^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:131:5`: `for` loops are no longer supported

  ```nextflow
      for (group in summary_params.keySet()) {
      ^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:131:10`: `group` is not defined

  ```nextflow
      for (group in summary_params.keySet()) {
           ^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:132:47`: `group` is not defined

  ```nextflow
          def group_params = summary_params.get(group)  // This gets the parameters of that particular group
                                                ^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:134:68`: `group` is not defined

  ```nextflow
              summary_section += "    <p style=\"font-size:110%\"><b>$group</b></p>\n"
                                                                     ^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:136:13`: `for` loops are no longer supported

  ```nextflow
              for (param in group_params.keySet()) {
              ^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:136:18`: `param` is not defined

  ```nextflow
              for (param in group_params.keySet()) {
                   ^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:137:49`: `param` is not defined

  ```nextflow
                  summary_section += "        <dt>$param</dt><dd><samp>${group_params.get(param) ?: '<span style=\"color:#999999;\">N/A</a>'}</samp></dd>\n"
                                                  ^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:137:89`: `param` is not defined

  ```nextflow
                  summary_section += "        <dt>$param</dt><dd><samp>${group_params.get(param) ?: '<span style=\"color:#999999;\">N/A</a>'}</samp></dd>\n"
                                                                                          ^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:284:5`: `for` loops are no longer supported

  ```nextflow
      for (group in summary_params.keySet()) {
      ^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:284:10`: `group` is not defined

  ```nextflow
      for (group in summary_params.keySet()) {
           ^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:285:34`: `group` is not defined

  ```nextflow
          summary << summary_params[group]
                                   ^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:344:42`: `GroovyException` is not defined

  ```nextflow
              if (plaintext_email) { throw GroovyException('Send plaintext e-mail, not HTML') }
                                           ^^^^^^^^^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:361:5`: `FilesEx` is not defined

  ```nextflow
      FilesEx.copyTo(output_hf.toPath(), "${outdir}/pipeline_info/pipeline_report.html");
      ^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:367:5`: `FilesEx` is not defined

  ```nextflow
      FilesEx.copyTo(output_tf.toPath(), "${outdir}/pipeline_info/pipeline_report.txt");
      ^^^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:392:5`: `for` loops are no longer supported

  ```nextflow
      for (group in summary_params.keySet()) {
      ^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:392:10`: `group` is not defined

  ```nextflow
      for (group in summary_params.keySet()) {
           ^^^^^
  ```

- Error: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:393:34`: `group` is not defined

  ```nextflow
          summary << summary_params[group]
                                   ^^^^^^^
  ```

- Error: `workflows/genealignment.nf:9:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/pipelines/genealignment/subworkflows/local/yaml_input.nf'

  ```nextflow
  include { YAML_INPUT             } from '../subworkflows/local/yaml_input'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:11:1`: Module could not be parsed: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/pipelines/genealignment/subworkflows/local/gene_alignment.nf'

  ```nextflow
  include { GENE_ALIGNMENT         } from '../subworkflows/local/gene_alignment'
  ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:45:5`: `YAML_INPUT` is not defined

  ```nextflow
      YAML_INPUT (
      ^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:54:9`: `YAML_INPUT` is not defined

  ```nextflow
          YAML_INPUT.out.reference_ch
          ^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:62:5`: `GENE_ALIGNMENT` is not defined

  ```nextflow
      GENE_ALIGNMENT (
      ^^^^^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:64:9`: `YAML_INPUT` is not defined

  ```nextflow
          YAML_INPUT.out.reference_ch,
          ^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:66:9`: `YAML_INPUT` is not defined

  ```nextflow
          YAML_INPUT.out.align_data_dir,
          ^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:67:9`: `YAML_INPUT` is not defined

  ```nextflow
          YAML_INPUT.out.align_geneset,
          ^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:68:9`: `YAML_INPUT` is not defined

  ```nextflow
          YAML_INPUT.out.intron_size,
          ^^^^^^^^^^
  ```

- Error: `workflows/genealignment.nf:71:39`: `GENE_ALIGNMENT` is not defined

  ```nextflow
      ch_versions     = ch_versions.mix(GENE_ALIGNMENT.out.versions)
                                        ^^^^^^^^^^^^^^
  ```

## :warning: Warnings

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

- Warning: `modules/nf-core/custom/getchromsizes/main.nf:26:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ''
          ^^^^
  ```

- Warning: `modules/nf-core/fastqc/main.nf:27:48`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      def renamed_files = old_new_pairs.collect{ old_name, new_name -> new_name }.join(' ')
                                                 ^^^^^^^^
  ```

- Warning: `modules/nf-core/paftools/sam2paf/main.nf:22:9`: Variable was declared but not used

  ```nextflow
      def args    = task.ext.args     ?: ""
          ^^^^
  ```

- Warning: `subworkflows/local/generate_genome.nf:15:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions     = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_genome.nf:16:5`: Variable was declared but not used

  ```nextflow
      ch_genomesize   = Channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/generate_genome.nf:16:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genomesize   = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/generate_genome.nf:17:5`: Variable was declared but not used

  ```nextflow
      ch_genome_fai   = Channel.empty()
      ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/generate_genome.nf:17:23`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_genome_fai   = Channel.empty()
                        ^^^^^^^
  ```

- Warning: `subworkflows/local/nuc_alignments.nf:27:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/nuc_alignments.nf:38:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .map { meta, nuc_file, ref_meta, ref, intron ->
                                 ^^^^^^^^
  ```

- Warning: `subworkflows/local/nuc_alignments.nf:145:19`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
          .filter { it[0].file_size >= 141 } // Take the first item in input (meta) and check if size is more than a symlink
                    ^^
  ```

- Warning: `subworkflows/local/nuc_alignments.nf:147:32`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { meta, ref, genome_meta, genome ->
                                 ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/pep_alignments.nf:22:27`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions         = Channel.empty()
                            ^^^^^^^
  ```

- Warning: `subworkflows/local/pep_alignments.nf:39:41`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          .multiMap { pep_meta, pep_file, miniprot_meta, miniprot_index ->
                                          ^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genealignment_pipeline/main.nf:38:5`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      input             //  string: Path to input samplesheet
      ^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genealignment_pipeline/main.nf:42:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genealignment_pipeline/main.nf:79:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genealignment_pipeline/main.nf:91:38`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              validateInputSamplesheet(it)
                                       ^^
  ```

- Warning: `subworkflows/local/utils_nfcore_genealignment_pipeline/main.nf:154:39`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
      def endedness_ok = metas.collect{ it.single_end }.unique().size == 1
                                        ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:121:48`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
                  .map { processVersionsFromYAML(it) }
                                                 ^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:123:22`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
                  .mix(Channel.of(workflowVersionToYAML()))
                       ^^^^^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:264:14`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      } catch (all) {
               ^^^
  ```

- Warning: `subworkflows/nf-core/utils_nfcore_pipeline/main.nf:350:18`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
          } catch (all) {
                   ^^^
  ```

- Warning: `workflows/genealignment.nf:31:19`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      ch_versions = Channel.empty()
                    ^^^^^^^
  ```

- Warning: `workflows/genealignment.nf:33:5`: The use of `Channel` to access channel factories is deprecated -- use `channel` instead

  ```nextflow
      Channel
      ^^^^^^^
  ```

- Warning: `workflows/genealignment.nf:79:16`: Variable was declared but not used

  ```nextflow
          .set { ch_collated_versions }
                 ^^^^^^^^^^^^^^^^^^^^
  ```
