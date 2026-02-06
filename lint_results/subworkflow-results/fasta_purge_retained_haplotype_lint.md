# Nextflow lint results

- Generated: 2026-02-06T13:21:24.477492+00:00
- Nextflow version: 25.12.0-edge
- Summary: 43 errors

## :x: Errors

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:6:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/cat/cat.nf'

    ```nextflow
    include { CAT_CAT as CONCATENATE_HAPLOTYPES         } from '../../../modules/nf-core/cat/cat'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:7:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/minimap2/align.nf'

    ```nextflow
    include { MINIMAP2_ALIGN as MINIMAP2_ALIGN_ASSEMBLY } from '../../../modules/nf-core/minimap2/align'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:8:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/purgedups/calcuts.nf'

    ```nextflow
    include { PURGEDUPS_CALCUTS                         } from '../../../modules/nf-core/purgedups/calcuts'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:9:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/purgedups/getseqs.nf'

    ```nextflow
    include { PURGEDUPS_GETSEQS                         } from '../../../modules/nf-core/purgedups/getseqs'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:10:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/purgedups/histplot.nf'

    ```nextflow
    include { PURGEDUPS_HISTPLOT                        } from '../../../modules/nf-core/purgedups/histplot'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:11:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/purgedups/pbcstat.nf'

    ```nextflow
    include { PURGEDUPS_PBCSTAT                         } from '../../../modules/nf-core/purgedups/pbcstat'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:12:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/purgedups/purgedups.nf'

    ```nextflow
    include { PURGEDUPS_PURGEDUPS                       } from '../../../modules/nf-core/purgedups/purgedups'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:13:1`: Invalid include source: '/home/runner/work/nextflow-strict-syntax-health/nextflow-strict-syntax-health/modules/modules/nf-core/purgedups/splitfa.nf'

    ```nextflow
    include { PURGEDUPS_SPLITFA                         } from '../../../modules/nf-core/purgedups/splitfa'
    ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:50:5`: `PURGEDUPS_PBCSTAT` is not defined

    ```nextflow
        PURGEDUPS_PBCSTAT(FASTX_MAP_LONG_READS.out.paf)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:51:35`: `PURGEDUPS_PBCSTAT` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(PURGEDUPS_PBCSTAT.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:56:5`: `PURGEDUPS_CALCUTS` is not defined

    ```nextflow
        PURGEDUPS_CALCUTS(PURGEDUPS_PBCSTAT.out.stat)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:56:23`: `PURGEDUPS_PBCSTAT` is not defined

    ```nextflow
        PURGEDUPS_CALCUTS(PURGEDUPS_PBCSTAT.out.stat)
                          ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:57:35`: `PURGEDUPS_CALCUTS` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(PURGEDUPS_CALCUTS.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:62:35`: `PURGEDUPS_PBCSTAT` is not defined

    ```nextflow
        ch_purgedups_histplot_input = PURGEDUPS_PBCSTAT.out.stat
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:63:18`: `PURGEDUPS_CALCUTS` is not defined

    ```nextflow
            .combine(PURGEDUPS_CALCUTS.out.cutoff, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:65:5`: `PURGEDUPS_HISTPLOT` is not defined

    ```nextflow
        PURGEDUPS_HISTPLOT(ch_purgedups_histplot_input)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:66:35`: `PURGEDUPS_HISTPLOT` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(PURGEDUPS_HISTPLOT.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:71:5`: `PURGEDUPS_SPLITFA` is not defined

    ```nextflow
        PURGEDUPS_SPLITFA(ch_assemblies_split.primary)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:72:35`: `PURGEDUPS_SPLITFA` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(PURGEDUPS_SPLITFA.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:77:5`: `MINIMAP2_ALIGN_ASSEMBLY` is not defined

    ```nextflow
        MINIMAP2_ALIGN_ASSEMBLY (
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:78:9`: `PURGEDUPS_SPLITFA` is not defined

    ```nextflow
            PURGEDUPS_SPLITFA.out.split_fasta,
            ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:89:26`: `PURGEDUPS_PBCSTAT` is not defined

    ```nextflow
        ch_purgedups_input = PURGEDUPS_PBCSTAT.out.basecov
                             ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:90:18`: `PURGEDUPS_CALCUTS` is not defined

    ```nextflow
            .combine(PURGEDUPS_CALCUTS.out.cutoff, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:91:18`: `MINIMAP2_ALIGN_ASSEMBLY` is not defined

    ```nextflow
            .combine(MINIMAP2_ALIGN_ASSEMBLY.out.paf, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:93:5`: `PURGEDUPS_PURGEDUPS` is not defined

    ```nextflow
        PURGEDUPS_PURGEDUPS(ch_purgedups_input)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:94:35`: `PURGEDUPS_PURGEDUPS` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(PURGEDUPS_PURGEDUPS.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:100:18`: `PURGEDUPS_PURGEDUPS` is not defined

    ```nextflow
            .combine(PURGEDUPS_PURGEDUPS.out.bed, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:102:5`: `PURGEDUPS_GETSEQS` is not defined

    ```nextflow
        PURGEDUPS_GETSEQS(ch_getseqs_input)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:103:35`: `PURGEDUPS_GETSEQS` is not defined

    ```nextflow
        ch_versions = ch_versions.mix(PURGEDUPS_GETSEQS.out.versions)
                                      ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:110:18`: `PURGEDUPS_GETSEQS` is not defined

    ```nextflow
            .combine(PURGEDUPS_GETSEQS.out.haplotigs, by: 0)
                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:125:5`: `CONCATENATE_HAPLOTYPES` is not defined

    ```nextflow
        CONCATENATE_HAPLOTYPES(ch_alt_split.concatenate)
        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:130:37`: `CONCATENATE_HAPLOTYPES` is not defined

    ```nextflow
        ch_alts = ch_alt_split.asis.mix(CONCATENATE_HAPLOTYPES.out.file_out)
                                        ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:133:34`: `PURGEDUPS_GETSEQS` is not defined

    ```nextflow
        purged_assemblies          = PURGEDUPS_GETSEQS.out.purged.combine(ch_alts, by: 0)
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:134:34`: `PURGEDUPS_GETSEQS` is not defined

    ```nextflow
        purged_haplotigs           = PURGEDUPS_GETSEQS.out.haplotigs
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:135:34`: `PURGEDUPS_SPLITFA` is not defined

    ```nextflow
        purgedups_splitfa          = PURGEDUPS_SPLITFA.out.split_fasta
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:136:34`: `MINIMAP2_ALIGN_ASSEMBLY` is not defined

    ```nextflow
        purgedups_splitfa_self_paf = MINIMAP2_ALIGN_ASSEMBLY.out.paf
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:137:34`: `PURGEDUPS_PBCSTAT` is not defined

    ```nextflow
        purgedups_pbcstat_hist     = PURGEDUPS_PBCSTAT.out.stat
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:138:34`: `PURGEDUPS_PBCSTAT` is not defined

    ```nextflow
        purgedups_pbcstat_basecov  = PURGEDUPS_PBCSTAT.out.basecov
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:139:34`: `PURGEDUPS_CALCUTS` is not defined

    ```nextflow
        purgedups_calcuts_cutoffs  = PURGEDUPS_CALCUTS.out.cutoff
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:140:34`: `PURGEDUPS_CALCUTS` is not defined

    ```nextflow
        purgedups_calcuts_log      = PURGEDUPS_CALCUTS.out.log
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:141:34`: `PURGEDUPS_HISTPLOT` is not defined

    ```nextflow
        purgedups_histplot         = PURGEDUPS_HISTPLOT.out.png
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:142:34`: `PURGEDUPS_PURGEDUPS` is not defined

    ```nextflow
        purgedups_bed              = PURGEDUPS_PURGEDUPS.out.bed
                                     ^^^^^^^^^^
    ```

- Error: `subworkflows/sanger-tol/fasta_purge_retained_haplotype/main.nf:143:34`: `PURGEDUPS_PURGEDUPS` is not defined

    ```nextflow
        purgedups_log              = PURGEDUPS_PURGEDUPS.out.log
                                     ^^^^^^^^^^
    ```
