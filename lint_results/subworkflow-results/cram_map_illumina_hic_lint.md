# Nextflow lint results

- Generated: 2026-02-06T13:21:24.474928+00:00
- Nextflow version: 25.12.0-edge
- Summary: 16 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:1:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/bwamem2/index/main.nf'

    ```nextflow
    include { BWAMEM2_INDEX              } from '../../../modules/nf-core/bwamem2/index/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:5:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/minimap2/index/main.nf'

    ```nextflow
    include { MINIMAP2_INDEX             } from '../../../modules/nf-core/minimap2/index/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:6:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/index/main.nf'

    ```nextflow
    include { SAMTOOLS_INDEX             } from '../../../modules/nf-core/samtools/index/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:7:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/samtools/splitheader/main.nf'

    ```nextflow
    include { SAMTOOLS_SPLITHEADER       } from '../../../modules/nf-core/samtools/splitheader/main'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:56:5`: `SAMTOOLS_INDEX` is not defined

    ```nextflow
        SAMTOOLS_INDEX(ch_hic_cram_raw.no_index)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:57:35`: `SAMTOOLS_INDEX` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(SAMTOOLS_INDEX.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:61:43`: `SAMTOOLS_INDEX` is not defined

    ```nextflow
                ch_hic_cram_raw.no_index.join(SAMTOOLS_INDEX.out.crai)
                                              ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:89:5`: `SAMTOOLS_SPLITHEADER` is not defined

    ```nextflow
        SAMTOOLS_SPLITHEADER(ch_hic_cram_meta_mod)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:90:35`: `SAMTOOLS_SPLITHEADER` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(SAMTOOLS_SPLITHEADER.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:92:21`: `SAMTOOLS_SPLITHEADER` is not defined

    ```nextflow
        ch_readgroups = SAMTOOLS_SPLITHEADER.out.readgroup
                        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:114:9`: `BWAMEM2_INDEX` is not defined

    ```nextflow
            BWAMEM2_INDEX(ch_assemblies)
            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:115:39`: `BWAMEM2_INDEX` is not defined

    ```nextflow
            ch_versions = ch_versions.mix(BWAMEM2_INDEX.out.versions)
                                          ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:119:22`: `BWAMEM2_INDEX` is not defined

    ```nextflow
                .combine(BWAMEM2_INDEX.out.index, by: 0)
                         ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:137:9`: `MINIMAP2_INDEX` is not defined

    ```nextflow
            MINIMAP2_INDEX(ch_assemblies)
            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:138:39`: `MINIMAP2_INDEX` is not defined

    ```nextflow
            ch_versions = ch_versions.mix(MINIMAP2_INDEX.out.versions)
                                          ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/cram_map_illumina_hic/main.nf:142:22`: `MINIMAP2_INDEX` is not defined

    ```nextflow
                .combine(MINIMAP2_INDEX.out.index, by: 0)
                         ^^^^^^^^^^
    ```
