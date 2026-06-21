# WGS Annotation of MDR *Pseudomonas aeruginosa* ST233

**Author:** Pareekshya Devkota  
**Institution:** Tri-Chandra Multiple Campus, Tribhuvan University  
**Date:** June 2026  
**ORCID:** [0009-0003-8645-0626](https://orcid.org/0009-0003-8645-0626)  
**NCBI SRA:** [SRR38675381](https://www.ncbi.nlm.nih.gov/sra/SRR38675381)  
**License:** MIT

---

## Overview

Whole genome sequence assembly and annotation of a clinical multidrug-resistant Pseudomonas aeruginosa ST233 isolate. ST233 is a clinically relevant lineage associated with MDR infections. This genome carries blaVIM-2 metallo-beta-lactamase alongside an OprD missense mutation (V359L), suggesting a dual carbapenem resistance mechanism consistent with reduced antibiotic uptake and enzymatic hydrolysis.

---

## Genome Statistics

| Property | Value |
|---|---|
| Sequence type | ST233 |
| Genome size | 6.87 Mb |
| Contigs | 431 |
| N50 | 89,636 bp |
| GC content | 66.2% |
| Coding density | 88.7% |
| CDSs | 6,221 |
| tRNAs | 68 |
| rRNAs | 3 |
| CRISPR arrays | 4 |

---

## AMR Profile

| Gene | Class | Mechanism |
|---|---|---|
| blaVIM-2 | Carbapenem | Metallo-beta-lactamase |
| blaOXA-486 | Beta-lactam | Oxacillinase |
| blaPDC-3 | Cephalosporin | AmpC beta-lactamase |
| oprD_V359L | Carbapenem | OprD porin missense mutation (identified via AMRFinder+ protein-level analysis against PAO1 reference) |
| sul1 | Sulfonamide | Target replacement |
| dfrB5 | Trimethoprim | Target replacement |
| aac(3)-Id | Aminoglycoside | Acetyltransferase |
| aac(6')-Il | Aminoglycoside | Acetyltransferase |
| aph(3')-IIb | Aminoglycoside | Phosphotransferase |
| catB7 | Chloramphenicol | Acetyltransferase |
| fosA | Fosfomycin | Glutathione transferase |
| gyrA_T83I | Fluoroquinolone | Target mutation |
| parC_S87L | Fluoroquinolone | Target mutation |
| nalC_G71E | Efflux regulation | Regulatory mutation |

**Acquired resistance genes:** blaVIM-2, blaOXA-486, blaPDC-3, sul1, dfrB5, aac(3)-Id, aac(6')-Il, aph(3')-IIb, catB7, fosA  
**Chromosomal mutations:** oprD_V359L, gyrA_T83I, parC_S87L  
**Regulatory mutations:** nalC_G71E

Carbapenem resistance involves dual mechanisms: enzymatic hydrolysis via blaVIM-2 and reduced outer membrane permeability via OprD V359L missense mutation. Fluoroquinolone resistance is conferred by target site mutations in both gyrA and parC, consistent with predicted high-level fluoroquinolone resistance. The genome carries resistance determinants spanning six antibiotic classes: beta-lactams, aminoglycosides, fluoroquinolones, sulfonamides, chloramphenicol, and fosfomycin, consistent with a broadly MDR phenotype.

---

## Methods

**Assembly:** Illumina paired-end reads assembled with SPAdes. Assembly quality assessed with QUAST (genome size 6.87 Mb, N50 89,636 bp, 431 contigs). Genome completeness confirmed with BUSCO (>99% expected for Pseudomonas aeruginosa).  
**Sequence typing:** MLST v2.35.0 against PubMLST Pseudomonas aeruginosa scheme.  
**Genome annotation:** Bakta v1.12.0 with light database (v6.0).  
**AMR detection:** AMRFinder+ v4.2.7 (database 2026-05-15.1, --organism Pseudomonas_aeruginosa).

---

## Repository Structure

    PA-ST233-WGS-annotation/
    ├── LICENSE
    ├── CITATION.cff
    └── results/
        ├── annotation/
        │   ├── SRR38675381.gff3      # Genome annotation
        │   ├── SRR38675381.tsv       # Annotation table
        │   ├── SRR38675381.txt       # Annotation summary
        │   └── SRR38675381.png       # Circular genome plot
        └── amrfinder/
            └── SRR38675381_amr.tsv   # AMRFinder+ results

---

## Contact

Pareekshya Devkota - devkotapareekshya08@gmail.com  
Tri-Chandra Multiple Campus, Tribhuvan University, Kathmandu, Nepal

## Related Repository

ST111 comparative OprD and AMR analysis: https://github.com/devkotapareekshya/PA-ST111-WGS-analysis
