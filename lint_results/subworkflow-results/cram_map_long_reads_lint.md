# Nextflow lint results

- Generated: 2026-02-06T13:21:24.475863+00:00
- Nextflow version: 25.12.0-edge
- Summary: 12 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:3:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/minimap2/index/main.nf'

    ```nextflow
    include { MINIMAP2_INDEX                  } from '../../../modules/nf-core/minimap2/index/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:4:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/index/main.nf'

    ```nextflow
    include { SAMTOOLS_INDEX                  } from '../../../modules/nf-core/samtools/index/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:5:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/splitheader/main.nf'

    ```nextflow
    include { SAMTOOLS_SPLITHEADER            } from '../../../modules/nf-core/samtools/splitheader/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:53:5`: `SAMTOOLS_INDEX` is not defined

    ```nextflow
        SAMTOOLS_INDEX(ch_cram_raw.no_index)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:54:35`: `SAMTOOLS_INDEX` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(SAMTOOLS_INDEX.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:58:39`: `SAMTOOLS_INDEX` is not defined

    ```nextflow
                ch_cram_raw.no_index.join(SAMTOOLS_INDEX.out.crai)
                                          ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:85:5`: `SAMTOOLS_SPLITHEADER` is not defined

    ```nextflow
        SAMTOOLS_SPLITHEADER(ch_crams_meta_mod)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:86:35`: `SAMTOOLS_SPLITHEADER` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(SAMTOOLS_SPLITHEADER.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:88:21`: `SAMTOOLS_SPLITHEADER` is not defined

    ```nextflow
        ch_readgroups = SAMTOOLS_SPLITHEADER.out.readgroup
                        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:106:5`: `MINIMAP2_INDEX` is not defined

    ```nextflow
        MINIMAP2_INDEX(ch_assemblies)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:107:35`: `MINIMAP2_INDEX` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(MINIMAP2_INDEX.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_long_reads/main.nf:111:18`: `MINIMAP2_INDEX` is not defined

    ```nextflow
            .combine(MINIMAP2_INDEX.out.index, by: 0)
                     ^^^^^^^^^^
    ```
