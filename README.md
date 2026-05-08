# QIIME2 Automated Microbiome Analysis Pipeline

This repository contains a fully automated QIIME2 workflow for microbiome analysis using paired-end 16S rRNA sequencing data.

The pipeline performs:

- Sequence import
- Quality filtering
- Dereplication
- OTU clustering (97%)
- Taxonomic classification using SILVA
- Taxa visualization
- Differential abundance analysis (ANCOM)
- Bray-Curtis beta diversity analysis

The goal of this pipeline is to simplify routine microbiome processing into a single reproducible workflow that can be executed with minimal manual intervention.

---

# Project Structure

```bash
project/
│
├── combined_analysis/              # Input FASTQ files
├── metadata_combined.tsv           # Sample metadata
├── results/                        # Generated outputs
├── qiime2_pipeline.sh              # Main pipeline script
│
├── silva-138-99-seqs.qza           # SILVA reference sequences
└── silva-138-99-tax.qza            # SILVA taxonomy database
