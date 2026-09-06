# Sanger Sequencing and Consensus Sequence Generation

## Overview

This project documents the analysis of bidirectional Sanger sequencing data to generate and validate a consensus nucleotide sequence.

The analysis was performed using CodonCode Aligner, starting from forward and reverse chromatogram files in AB1 format.

## Objectives

- Inspect the quality of forward and reverse Sanger chromatograms.
- Identify low-quality regions and poorly resolved signals.
- Evaluate peak clarity and separation.
- Correct unreliable base calls when supported by chromatogram evidence.
- Generate and validate a consensus nucleotide sequence.
- Export the final consensus sequence in FASTA format.

## Workflow

Forward chromatogram (.ab1)
+
Reverse chromatogram (.ab1)
↓
Quality assessment
↓
Trimming of low-quality regions
↓
Chromatogram inspection
↓
Base-call correction
↓
Comparison of forward and reverse reads
↓
Consensus generation
↓
Consensus validation
↓
FASTA export

## Sample

Sample ID: A5-2021-06-25

Final consensus length: 773 bp

## Quality Assessment

The forward and reverse chromatograms were inspected separately.

### Forward read

- The beginning of the read showed poorly resolved peaks and limited peak separation.
- Peak resolution improved in the region approximately between bases 70 and 130.
- Toward the end of the read, peak intensity progressively decreased, indicating a decline in signal quality.

### Reverse read

- The beginning of the read showed poor peak separation, overlapping signals, and irregular peaks.
- Peak resolution improved in the middle region of the read.
- Toward the end, the peaks became weaker and less well separated, with overlapping signals.

Detailed observations are provided in:

`results/Sanger_Chromatogram_Quality_Assessment.xlsx`

## Final Consensus

The final consensus sequence is provided in:

`consensus/A5_2021-06-25_consensus.fasta`

## Tools

- CodonCode Aligner
- Sanger sequencing chromatograms (AB1)
- FASTA format
- Excel for quality assessment

## Project Status

Completed
