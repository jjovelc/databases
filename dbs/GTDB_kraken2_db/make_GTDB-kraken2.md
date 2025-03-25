# How to build a GTDB kraken2 DB

GTDB (Genome Taxonomy Database) does not provide full genome sequences directly. GTDB classifies genomes, but the actual genomic sequences come from external sources, primarily NCBI GenBank / RefSeq. Thus, GTDB is built on genomes from GenBank, RefSeq, and some MAGs (metagenome-assembled genomes). GTDB keeps only metadata, taxonomy, and protein alignments, not the raw genome files.

1. Create appropriate directory and dowload metadata from GTDB

```bash
  mkdir kraken2_gtdb220_genbank_250325
  cd kraken2_gtdb220_genbank_250325
  wget https://data.gtdb.ecogenomic.org/releases/latest/ar53_metadata.tsv.gz
  wget https://data.gtdb.ecogenomic.org/releases/latest/bac120_metadata.tsv.gz
  gunzip *.gz
```

2. 

   
