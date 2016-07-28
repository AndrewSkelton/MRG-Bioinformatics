# MRG-Bioinformatics
List of Complete Bioinformatics work

---

## Louise Reynard
### Methylation Collaboration Project - Time Commitment ~1.5 Days
* Scripps Transcription Factor Enrichment Analysis
* Mandy Transcription Factor Enrichment Analysis
  * MSC - chondrocyte
  * MSC - OB
  * MSC - Tenocyte
  * Subset for Final CpG list for original collaboration
* Followup Enrichment analysis (TXF/ ENCODE Chromatin) for DM lists

### GEO Data request - Time Commitment ~0.15 Days
* Query and Get IDAT files for GSE80071
  * Archive Data
  * Get GEO Phenotype entry to match IDATs
* Query and Get IDAT files for GSE46364
  * Requires collaboration to share IDAT files

### Data Queries - Time Commitment ~0.25 Days
* Gene Expression Query from Arthur's Datasets - CD4+/CD8+ for CHST11
* Genotype Query from Arthur's Datasets - See email for list

---

## Stuart Watson
### Methylation Arrays - Time Commitment ~1.25 Day
* Report results of non-linear effects
* Methods Section writing - Kelly

---

## Faye Cooles
### NanoString - Time Commitment ~2 Days
* Design model for experimental design
* Assess suitability of DESeq2 as analysis framework for NanoString Data
* Develop Contrasts
* Visualisations
* Export Results
* Discuss results and plan follow up work / analyses

---

## Sophie Hambleton
### PID Exome Project - Time Commitment ~1.5 Days
* Re-label mixed samplesqst
* Change ReadGroups - Easier to run preprocessing.
* Implement check for Missing bam files for a given sample map element
* Fix bug in pedigree reporting
  * Split for Families and singletons
  * Issue with sex allocation resolved
  * Gender issue with spaces in Sample Map (implemented in bash)
* 22nd July - Gender Issue on remapped samples - Still Issues, waiting on relatedness check.
  * Samples D180850,GNB051015,GNB120815,NG002,NG003,NG008,NG009 Appear to be wrong post re-label
  * Informed Jon - Waiting for confirmation to send MT Bams
  * Remapping was interpreted the opposite way around
  * Re-Labeled, Applying preprocessing
* Create test that checks relatedness against known pedigrees



---

## Colin Shepherd
### Data request - Time Commitment ~0.60 Days
* NOF OA RNA Seq data for genes of interest
  * Find transcript ID to gene ID mappings
  * Get TPMs
  * Get Gene Level normalised counts
  * Create output (openxlsx)
  * Send results
  * Additional Gene for Extraction (ALDH1A2)
  * Plotting advice and quick coding

---

## John Loughlin
### arcOGEN Data - Time Commitment ~0.6 Days
* Phenotype data requested
* Imputed (1000G Phase 1, GRCh37 Assembly) Data requested
* Data sent through via Globus Online
  * Phenotype Data - Split into two stages
  * Imputed Plink files (fam bed bim), 1000G P1 hg19
* Followup Britt - Phenotype FTP error

---

## Amanda Villalvilla
### arcOGEN Data Queries - Time Commitment ~0.35 Days
* SNP List Extract using Plink / R
  * Create SNP list from email
  * Subset Plink files, create transposed matrix of genotypes
    * Use Plink 1.9 on Sulaco
  * Send Results

---

## Fai Ng
### MSc Supervision - Time Commitment ~6 Days
* Weekly meeting to assess progress and guide
* Low Frequency support

---

## Jess Tarn
### PSS Datasets - Time Commitment ~0.25 Days
* Normalised, not batch corrected dataset
  * Validation set
  * Discovery set
  * Add to shared drive (pss_archive)

---

## Arthur Pratt
### T-Cell Dataset - Time Commitment ~1.75 Days
* eQTL of ~1000 Genes (ranked by variability)
* Interaction effect research
  * Try Multinomial Log-linear Model for i ~ x * y (i = Disease, x = GE, y = Geno)
  * Implement Logistic regression approach
  * Run over 7,000 gene expression probes ranked by variance
    * Ran over 1,000 probes with low variance - 3 Results, Variance rank seems to work.
  * Parallelise (40 Threads on Sulaco overnight - ~8Hrs)
  * Plot top results
    * 15,760,003 Tests - Could be limited using LD and MAF
    * 4 Pass FDR (Not convincing)
    * 67 (-4) P < 0.0001
    * Limited on Power due to Genotype, Disease Split
  * Meeting Friday 2pm

---

# Adrian Falconer
### HT12 Experiment - Time Commitment ~1.25 Days
* Experimental Design Meeting 2pm 25th July 2016
* Prep Data from IDAT -> S|CPP
* QC
* DE Analysis - Between TPs for each Sample Type
* DE Results (Padj < 0.05 & LFC > 2)
* Create Report in Markdown
  * Compile to PDF

---
