# Day 1 — Antimicrobial Resistance Basics

## 1. What is Antimicrobial Resistance?

Antimicrobial resistance (AMR) occurs when microorganisms such as bacteria develop the ability to survive or continue growing in the presence of an antimicrobial drug that would normally inhibit or kill them.

AMR can make infections more difficult to treat because some antimicrobial drugs may no longer work effectively.

---

## 2. Antimicrobials and Antibiotics

Antimicrobials are drugs or substances used to prevent or treat infections caused by microorganisms. Antibiotics specifically act against bacteria.


---

## 3. How Does Bacterial Resistance Develop?

Bacteria can acquire resistance through:

* Mutations in their DNA
* Acquisition of resistance genes from other bacteria

Resistance genes can sometimes be transferred between bacteria through horizontal gene transfer. when the pathogen is exposed to the antimicrobial compund it starts to yndergo changes to confer the genes which are resistant and then passes these genes down vertically to generation to gerneration

Important mechanisms of horizontal gene transfer include:

* Transformation
* Transduction
* Conjugation

---

## 4. Major Mechanisms of Antibiotic Resistance

Bacteria can resist antibiotics in several ways.

### A. Drug inactivation

The bacterium produces an enzyme that chemically modifies or destroys the antibiotic.

Example: Beta-lactamases can break down beta-lactam antibiotics. beta -lactam antibiotics binds to the pencillin binding proteins (pbp) which are enzymes involved in cross-linking peptidoglycan strands during bacterial cell wall synthesis and makes the cell wall weak and unstable As a result, the bacterium can eventually lyse and die, especially when it is growing and dividing. This is why β-lactam antibiotics are called cell-wall synthesis inhibitors.

### B. Modification of the drug target

The antibiotic normally binds to a specific bacterial target. Changes to that target can reduce antibiotic binding and make the drug less effective.

### C. Reduced drug uptake

Changes in the bacterial cell envelope can reduce the amount of antibiotic entering the cell.

### D. Efflux pumps

Bacteria can use transport proteins called efflux pumps to remove antibiotics from the cell.

### E. Alternative metabolic pathways

A bacterium may develop or acquire another pathway that allows an important cellular process to continue even when the antibiotic blocks the original pathway.

---

## 5. Resistance Genes

A resistance gene is a gene whose product can contribute to resistance against an antimicrobial.

For example, some genes encode enzymes that inactivate antibiotics, while others encode altered drug targets or efflux systems.

In genome analysis, detecting a resistance-associated gene can provide evidence that the genome contains a genetic determinant associated with resistance.

However, detection of a resistance gene does not automatically prove that the bacterium is phenotypically resistant. Phenotypic resistance is normally determined using antimicrobial susceptibility testing.

---

## 6. Klebsiella pneumoniae

Klebsiella pneumoniae is a Gram-negative bacterium that can cause infections in humans.

It is important in antimicrobial-resistance research because some K. pneumoniae isolates contain multiple resistance determinants and can show resistance to several classes of antibiotics.

My project focuses on comparing the antimicrobial-resistance determinants found in publicly available K. pneumoniae genomes.

---

## 7. AMR Gene Detection

The basic idea of AMR gene detection is to examine a bacterial genome and identify genes or genetic determinants associated with antimicrobial resistance.

For my project, I will use computational tools to identify AMR determinants in publicly available K. pneumoniae genomes.

One important tool I will learn to use is NCBI AMRFinderPlus.

---

## 8. What is AMRFinderPlus?

AMRFinderPlus is an NCBI tool used to identify antimicrobial-resistance genes and other relevant resistance-associated determinants in microbial genome sequences.

It compares genomic sequences against curated information about known antimicrobial-resistance determinants.

The output can provide information such as the detected gene or protein, its associated antimicrobial class or mechanism, and other annotation information.

---

## 9. AMR Profiles

An AMR profile describes the collection of antimicrobial-resistance determinants detected in a particular bacterial genome.

For example:

Genome A → gene A + gene B
Genome B → gene A + gene C
Genome C → gene B + gene C

These profiles can be converted into a presence/absence matrix.

| Genome   | Gene A | Gene B | Gene C |
| -------- | -----: | -----: | -----: |
| Genome A |      1 |      1 |      0 |
| Genome B |      1 |      0 |      1 |
| Genome C |      0 |      1 |      1 |

Here, `1` means the determinant was detected and `0` means it was not detected.

This type of matrix will later be useful for comparing AMR profiles among K. pneumoniae genomes.

---

## 10. Why AMR Profiles Are Useful in My Project

Different K. pneumoniae genomes may contain different combinations of resistance determinants.

By comparing these profiles across multiple genomes, I can investigate how AMR determinants vary among the genomes in my dataset.

Later in the project, I will compare these AMR profiles with genomic/phylogenetic relationships.

A phylogenetic tree represents genomic relationships among isolates, while the AMR matrix represents their detected resistance determinants. Comparing the two can help describe whether particular AMR profiles are associated with particular genomic groups.

This comparison does not by itself prove that a particular lineage caused or acquired a resistance trait.

---

## 11. My Project Workflow

The basic workflow of my project is:

Klebsiella pneumoniae genomes
↓
Obtain genomes from NCBI
↓
Detect AMR determinants
↓
Create an AMR gene table
↓
Create a presence/absence matrix
↓
Analyze AMR profiles using Python
↓
Construct a phylogenetic tree
↓
Compare AMR profiles with genomic relationships
↓
Visualize and interpret the results

---

## 12. Important Distinction

There is an important difference between:

**AMR genotype:**
Resistance-associated genes or mutations detected in the genome.

**AMR phenotype:**
The actual observed response of the bacterium to an antimicrobial, usually determined through antimicrobial susceptibility testing.

My project primarily studies the genomic determinants of resistance. Therefore, I should not automatically describe a genome as phenotypically resistant just because a resistance-associated gene was detected.

---




