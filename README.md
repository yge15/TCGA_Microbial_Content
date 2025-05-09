# TCGA Microbial Content
Comprehensive analysis of microbial content in 5,734 whole-genome sequencing samples from The Cancer Genome Atlas project

These are the supplementary files and tables for our [bioRxiv preprint](https://www.biorxiv.org/content/10.1101/2024.05.24.595788v3.full.pdf) [1]
We are posting the files here because some of them are too large for the journal to take as supplements.

## Supplementary Tables Captions

1. Table S1. Overview of 569 solid tissue normal samples out of the 5,734 WGS samples analyzed in this study. Column headers are the same as for Table 1.
2. Table S2. Overview of 2,277 blood-derived normal samples out of the 5,734 WGS samples analyzed in this study. Column headers are the same as for Table 1.
3. Table S3. Raw counts of 5,734 TCGA WGS samples classified at the species level against the Kraken Microbial2023 database, excluding eukaryotes. The contents of Microbial2023 are described in the main text. This resulted in 11,332 species that have non-zero counts.
4. Table S4. Normalized counts of the values in Table S3, converted to counts per million reads sequenced.
5. Table S5. Raw counts of 5,734 TCGA WGS samples classified at the species level against Fungi_RefSeq database. The contents of Fungi_RefSeq include all 557 fungal species in RefSeq as of late 2023.
6. Table S6. Normalized counts of Table S5, converted to counts per million reads sequenced.
7. Table S7. TCGA study abbreviations.
8. Table S8. Raw counts of 18 selected viruses identified in each of 5,734 TCGA WGS samples by the TCGA project. The TCGA filtering process used bwa to align reads against a database including the human genome plus multiple strains of human papillomavirus (HPV), hepatitis B and C viruses (HBV, HCV-1 1, and HCV-2), and cytomegalovirus (CMV). Counts here include the 14 strains of HPV most often associated with cancer: 16, 18, 31, 33, 35, 39, 45, 51, 52, 56, 58, 59, 66, and 68. Unlike the counts from Kraken2, which treated paired reads as a unit, paired reads were counted separately here; thus if both reads in a pair aligned, this was counted as 2 matches. Note that unlike the KrakenUniq database, low-complexity sequences were not masked out prior to alignment, which might have yielded many false-positive matches for some viruses.
9. Table S9. Raw counts of 4,550 TCGA WGS samples classified at the genus level against Microbial2023 database, for samples used in both this study and in the Poore et al. study. This dataset contains counts for all 3,563 genera that had non-zero counts in either study.
10. Table S10. Raw counts from the Poore et al. study at the genus level, for samples used in both this study and Poore et al. This set contains 4,550 samples and 3,563 genera. Raw counts included here were taken directly from Poore et al. (2020).
11. Table S11. Raw counts of TCGA WGS samples classified at the species level against the Fungi_RefSeq database, for samples and species matched with the Narunsky-Haziza et al. study. This resulted in 4,271 samples and 224 species.
12. Table S12. Raw counts from the Narunsky-Haziza et al. study at the species level, for samples and species matched with this study. This resulted in 4,271 samples and 224 species. Raw counts included here were taken directly from Narunsky-Haziza et al. (2022).
13. Table S13. TCGA metadata for 5,734 samples, including unique IDs for this study, IDs used by Poore et al., IDs used by Narunsky-Haziza et al., and the original TCGA identifiers.
14. Table S14. List of species in the Microbial2023 Kraken database, with RefSeq accessions. Note that for the purposes of future analysis, some of these species might be combined, using the species-level counts in Table S1. For example, the database contains 15 different species and 63 genomes from the genus Fusobacterium, and more than one of these has been reported to be present in the colon.
15. Table S15. List of species in the Fungi_RefSeq Kraken database, with RefSeq accessions.
16. Table S16. RefSeq v200 to v220 name conversion list, for 14 of the 557 fungal species whose names were changed between the two releases of RefSeq.


## Citation
1. Ge, Y., Lu, J., Puiu, D., Revsine, M., & Salzberg, S. L. (2024). Comprehensive analysis of microbial content in whole-genome sequencing samples from The Cancer Genome Atlas project. bioRxiv, 2024-05.

## Updates
1. 19 August 2024: We have updated Table S1-3 and S9-10 by removing raw counts related to HPV, HBV/HCV, and CMV, and added Table S5 separately for those viral counts.
2. 16 March 2025: For consistency and correctness, we added back the reads previously aligned to HPV, HBV, HCV-1, HCV-2, and CMV into our Kraken analysis. Those new viral reads were reported in the updated Table S1 and S2. The tables normalized by per kilobase of genome were removed.
3. 23 April 2025: Due to reviewer's request, we have added three more columns to TableS13_Metadata-Enhanced. These columns headers are Sequencing_Center, Sequencing_Date, and Center_id.
4. 9 May 2025: We added two more Supplentary Tables S1 and S2 for solid tissue normal and blood-derived normal samples; Table 1 in the main text was revised to represent primary tumor samples only.
