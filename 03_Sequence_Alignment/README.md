# Project 3 — Sequence Alignment

## Overview

This project looks at nucleotide and protein sequence alignment. The human **TP53** gene is used as a model. The goal is to compare sequences from different species, find conserved regions and differences, and understand what they mean in biology.

## Objectives

- Download nucleotide and protein sequences from NCBI.
- Do a pairwise alignment of the nucleotide sequences.
- Check the sequence identity, the query coverage, and how significant the alignment is.
- Look at conserved regions, substitutions, and gaps.
- Repeat the analysis with protein sequences.
- Explain the results and write them down.

## Part 1 — Nucleotide Sequence Alignment

### Sequences

| Organism | Gene | Accession | Region used |
|---|---|---|---|
| Human (*Homo sapiens*) | TP53 | NM_000546.6 | CDS, positions 143–1324 |
| Chimpanzee (*Pan troglodytes*) | TP53 | XM_016931470.3 | CDS, positions 208–1443 |

**Data source:** NCBI RefSeq.

**Important note about the annotation:** The chimpanzee sequence is a predicted RefSeq transcript (the accession starts with `XM_`). Keep this in mind when reading the results.

### Method

The nucleotide alignment was done with NCBI BLASTN. I used the option **Align two or more sequences** and the **Megablast** algorithm. Megablast is made for sequences that are very similar.

### Results

| Metric | Result |
|---|---:|
| Percent identity | 99.55% |
| Query coverage | 94% |
| Alignment score | 2,017 bits |
| E-value | 0.0 |
| Identical positions | 1,103 / 1,108 |
| Gaps | 2 / 1,108 |
| Query length (reported by BLAST) | 1,180 nt |
| Subject length (reported by BLAST) | 1,236 nt |

### Preliminary Interpretation

The human and chimpanzee TP53 sequences are very similar in the aligned region. The identity is 99.55%, which shows strong conservation.

The alignment also has a few positions that are not identical, and two gaps. We must check these carefully before calling them substitutions, insertions, or deletions.

### Limitations

- The human CDS positions 143–1324 give 1,182 nucleotides, but BLAST reports a query length of 1,180 nt. This difference is not explained yet.
- The chimpanzee sequence is predicted. It is not a curated `NM_` RefSeq transcript.
- The query coverage is 94%, so the alignment does not cover the whole query sequence.
- The alignment alone cannot show the functional effect of the differences.

These limits will be considered in the final interpretation.

## Part 2 — Protein Sequence Alignment

**Status:** To be completed.

The next step is to compare the TP53 protein sequences. This will show which amino acids are conserved and which are different between the species.

## Tools and Resources

- NCBI Nucleotide and RefSeq
- NCBI BLASTN
- FASTA sequence format

## Project Status

- [x] Download the human TP53 CDS
- [x] Download the chimpanzee TP53 CDS
- [x] Do the pairwise nucleotide alignment
- [x] Record the first alignment statistics
- [ ] Finish the interpretation of the nucleotide alignment
- [ ] Do the protein sequence alignment
- [ ] Compare nucleotide and protein conservation
- [ ] Finish the project documentation
