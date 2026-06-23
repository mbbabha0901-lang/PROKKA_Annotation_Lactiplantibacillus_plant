# PROKKA_OUTPUT

## Overview

This repository contains genome annotation results generated using Prokka from a de novo assembled genome of *Lactiplantibacillus plantarum*.

The genome assembly was obtained using SPAdes and subsequently annotated using Prokka v1.15.6. The repository includes predicted coding sequences, protein sequences, annotation files, and summary statistics.

---

## Software Used

- Prokka v1.15.6
- BLAST+ v2.16.0
- SPAdes
- QUAST

---

## Workflow

```text
Raw Reads
   │
   ▼
SPAdes Assembly
   │
   ▼
contigs.fasta
   │
   ▼
QUAST Assessment
   │
   ▼
Prokka Annotation
   │
   ▼
Annotated Genome
```

---

## Prokka Command

```bash
prokka contigs.fasta \
--outdir genannotat_lp \
--prefix lactiplanti \
--genus Lactiplantibacillus \
--species plantarum
```

---

## Output Files

| File | Description |
|------|-------------|
| lactiplanti.gff | Genome annotation in GFF3 format |
| lactiplanti.gbk | GenBank format annotation |
| lactiplanti.faa | Predicted protein sequences |
| lactiplanti.ffn | Nucleotide sequences of genes |
| lactiplanti.fna | Genome nucleotide sequences |
| lactiplanti.tsv | Annotation summary |
| lactiplanti.txt | Annotation statistics |

---

## Citation

Seemann T. (2014). *Prokka: Rapid prokaryotic genome annotation*. Bioinformatics, 30(14), 2068–2069.
