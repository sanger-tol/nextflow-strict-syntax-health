# Nextflow lint results

- Generated: 2026-10-08T15:35:39.711749112Z
- Nextflow version: 26.09.2-edge
- Summary: 7 warnings

## :warning: Warnings

- Warning: `modules/nf-core/binette/main.nf:59:9`: Variable was declared but not used

  ```nextflow
      def args = task.ext.args ?: ''
          ^^^^
  ```

- Warning: `subworkflows/local/bin_taxonomy/main.nf:15:5`: Variable was declared but not used

  ```nextflow
      ch_gtdb_merged_summary = channel.empty()
      ^^^^^^^^^^^^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/binning_vamb/main.nf:86:58`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_vamb_multi_bins = ch_vamb_multi.map { meta, bins, abundance, composition, vamb_log, taxometer, latent ->
                                                           ^^^^^^^^^
  ```

- Warning: `subworkflows/local/binning_vamb/main.nf:86:69`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_vamb_multi_bins = ch_vamb_multi.map { meta, bins, abundance, composition, vamb_log, taxometer, latent ->
                                                                      ^^^^^^^^^^^
  ```

- Warning: `subworkflows/local/binning_vamb/main.nf:86:82`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_vamb_multi_bins = ch_vamb_multi.map { meta, bins, abundance, composition, vamb_log, taxometer, latent ->
                                                                                   ^^^^^^^^
  ```

- Warning: `subworkflows/local/binning_vamb/main.nf:86:92`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_vamb_multi_bins = ch_vamb_multi.map { meta, bins, abundance, composition, vamb_log, taxometer, latent ->
                                                                                             ^^^^^^^^^
  ```

- Warning: `subworkflows/local/binning_vamb/main.nf:86:103`: Parameter was not used -- prefix with `_` to suppress warning

  ```nextflow
      ch_vamb_multi_bins = ch_vamb_multi.map { meta, bins, abundance, composition, vamb_log, taxometer, latent ->
                                                                                                        ^^^^^^
  ```
