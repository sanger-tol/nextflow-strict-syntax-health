# Nextflow lint results

- Generated: 2026-08-20T00:08:18.362980165Z
- Nextflow version: 26.07.0-edge
- Summary: 2 warnings

## :warning: Warnings

- Warning: `subworkflows/local/merge_output.nf:21:107`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [meta + [id: meta.specimen + ".merged_${params.merge_output}", merge_source: sorted.collect { it[0] }.join("\n") + "\n", read_count: read_counts.sum()], sorted.collect { it[1] }]
                                                                                                            ^^
  ```

- Warning: `subworkflows/local/merge_output.nf:21:183`: Implicit closure parameter is deprecated, declare an explicit parameter instead

  ```nextflow
              [meta + [id: meta.specimen + ".merged_${params.merge_output}", merge_source: sorted.collect { it[0] }.join("\n") + "\n", read_count: read_counts.sum()], sorted.collect { it[1] }]
                                                                                                                                                                                        ^^
  ```
