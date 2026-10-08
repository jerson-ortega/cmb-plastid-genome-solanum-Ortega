# Plastid Genome Lab Activity

## Student & Course Information

* **Student Name:** Jerson Llpyd T. Ortega
* **Course and Section:** Cell and Molecular Biology

## Organism & Accession Details

* **Chosen Genus & Species:** *Solanum lycopersicum* (Tomato)
* **NCBI Accession / Version:** NC_007898.3
* **NCBI Reference Link:** [https://www.ncbi.nlm.nih.gov/nuccore/NC_007898.3](https://www.ncbi.nlm.nih.gov/nuccore/NC_007898.3)
* **Retrieval Date:** September 29, 2026

## Plastome Overview & Size

* **Genome Size:** 155,461 base pairs (bp)
* **Plastome Summary:** The chloroplast genome shows a quadripartite plant structure containing Large Single Copy (LSC), Small Single Copy (SSC), and two Inverted Repeat (IR) regions, characterized by duplicated gene sets and standard plastid functional groups (photosystem subunits, ATP synthases, ribosomal proteins, rRNAs, and tRNAs).

## Methodology & Workflow

* **Acquisition:** The annotation file FASTA and GenBank were retrieved directly from NCBI RefSeq and processed locally.
* **R Environment & Tools Used:**
  * **Tools used:** Base R was utilized to compute basic sequence length, nucleotide composition, and summary metrics. A custom script (`01_genome_analysis.R`) parsed the `sequence.gb.txt` file to specifically extract gene features, calculate GC content, and build tabular summaries for analysis.

## Gene Content Summary and Observations

* **Total Gene Count:** ~114 unique genes (approx. 131 including duplicates).
* **Functional Group Breakdown:**
  * **Protein-Coding & Other Genes:** 80 (including *psa, psb, pet, rpo, rpl, rps,* and *ycf*).
  * **tRNA Genes:** 30.
  * **Ribosomal RNA (rRNA) Genes:** 4.
* **Notable Features:** Structural regions (LSC, SSC, IR) are defined by coordinate boundaries and duplicated gene blocks rather than explicit layout rows. Introns and exons are identifiable via associated exon and Parent tags.

## References

* National Center for Biotechnology Information (NCBI). *NCBI Reference Sequence NC_007898.3: Solanum lycopersicum chloroplast, complete genome.* U.S. National Library of Medicine. [https://www.ncbi.nlm.nih.gov/nuccore/NC_007898.3](https://www.ncbi.nlm.nih.gov/nuccore/NC_007898.3)
* Kahlau, S., Aspinall, S., Gray, J. C., & Bock, R. (2006). Sequence of the tomato chloroplast DNA and evolutionary comparison of solanaceous plastid genomes. *Journal of Molecular Evolution*, 63(2), 194-207.

## Reproducibility Guide

To replicate this analysis in R:

1. Import the *Solanum lycopersicum* chloroplast annotation file (`sequence.gb.txt`) into your local `data/raw/` directory.
2. Run the `01_genome_analysis.R` script with the condition to check sequence properties.
3. Review the terminal outputs to compute the GC content and filter the genes using appropriate variables.
4. Look for related studies to anchor it with your initial results.
   
