# BLAST Analysis of Genomic DNA of Human TP53

## Project Overview

This project investigates the human TP53 genomic DNA sequence using BLASTN and the NCBI nucleotide database.

The objective is to identify similar sequences, evaluate alignment statistics, examine genomic coordinates, and relate the main alignment to annotated TP53 genomic features.

## Query Sequence

- **Gene:** TP53 (tumor protein p53)
- **Organism:** Homo sapiens
- **Query length:** 19,088 bp
- **Analysis tool:** NCBI BLASTN (MegaBLAST)

## Project Structure

- `data/query/`: Query sequence used for the analysis.
- `data/references/`: Reference data.
- `results/BLAST_TP53_top_hits.md`: Summary of the top BLAST hits.
- `results/BLAST_TP53_alignment_analysis.md`: Main alignment statistics and biological interpretation.
- `results/BLAST_TP53_genomic_feature_mapping.md`: Mapping of the alignment to annotated TP53 genomic features.

## Main Findings

The main human TP53 reference hit, accession NG_017013.2, showed 100% query coverage, approximately 99.75% sequence identity, and an E-value of 0.0.

The analysis also identified other highly similar sequences, including a mouse chromosome 17 sequence and a partial match to WRAP53. These results require careful interpretation and comparison with the relevant genomic annotations.

## Conclusion

This project demonstrates the use of BLASTN to investigate genomic sequence similarity, evaluate alignment quality, and explore the genomic context of the human TP53 gene.

The findings support a strong correspondence between the query and the human TP53 genomic region. Sequence differences and cross-species matches must be interpreted in their appropriate biological context.
