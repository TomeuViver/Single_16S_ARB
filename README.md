# Taxonomic Analysis Based on Individual 16S rRNA Gene

## Description

In this workshop, we will learn how to use the bioinformatics program **ARB** for phylogenetic reconstruction based on the **16S rRNA gene**. ARB is a powerful software suite designed for handling and analyzing large sequence datasets, particularly in microbial taxonomy. We will use the **Living Tree Project ([LTP](https://imedea.uib-csic.es/mmg/ltp/)) database** as a reference, which provides a curated and phylogenetically structured dataset of 16S rRNA gene sequences from type strains of prokaryotic species.

The objective of this session is to:
- Learn how to integrate new sequences into the LTP database.
- Reconstruct a **phylogenetic tree** based on 16S rRNA sequences.
- Perform taxonomic classification using the ARB toolset.

This session will provide valuable hands-on experience in computational microbial taxonomy, which is essential for identifying and classifying novel bacterial and archaeal species.

## The Living Tree Project (LTP) Database

The **Living Tree Project (LTP) database** is a curated database containing aligned **16S rRNA gene sequences** from type strains of described bacterial and archaeal species. It is an essential reference for taxonomic studies and phylogenetic reconstructions.

### Downloading the Latest LTP Database

To download the most recent release of the **LTP database**, use the following command in the terminal:

```bash
wget 'https://disc-genomics.uibk.ac.at/data/LTP_10_2024.arb'
```

You can also visit the official [LTP website](https://imedea.uib-csic.es/mmg/ltp/) for further details about the database and updates.

## Using ARB for Phylogenetic Reconstruction

### Locating the 16S rRNA Gene Sequences

For this workshop, the **16S rRNA gene sequence** that we will use is stored in the following directory. Navigate to the folder using:

#### Open a terminal!!

#### Download the 16S rRNA sequence using:

```bash
wget  --content-disposition https://figshare.com/ndownloader/files/53160257
mv Salinibacter_16S.fasta.txt Salinibacter_16S.fasta
```

The file containing the 16S rRNA sequence is called Salinibacter_16S.fasta

Take a look to the 16S rRNA sequence:

```bash
less Salinibacter_16S.fasta
```

### 16S rRNA sequence 

```bash
>16S_rRNA_MAG
ACGGAGAGTTTGATCCTAGCTCAGGACGAACGCTGGCGGCAGGCTTAACACATGCAAGTCGCACGAGAACGTTCTGGCTTTGCCAG
AACAAGTACACTGGCGGACGGGTGCGTAACGCGTATATAACCTGCCTTCAGGCGCGGGACAACCTCGGGAAACCGTGGCTAATACC
GCACGACGTCCAGACCCCTCATGGGGACTGGATGAAAGCCTTATGGTGCCTGAAGATGGGTATGCGTCGGATTAGCTTGTTGGTGG
GGTAACGGCTCACCAAGGTAACGATCCGTAACTGGTCTGAGAGGATGATCAGTCACACTGGGACTGAGATACGGCCCAGACTCCTA
CGGGAGGCAGCAGTGGGGAATCTTGCACAATGGGGGAAACCCTGATGCAGCCATGGCGCGTGGAGGAAGACACCCCTATGGGGCGT
AAACTCCTTTTCTGCGCGAAGAAACCTCTGTTTTTCAGAGTGTGACGGTACCGCAGGAATAAGGACCGGCTAACTCCGTGCCAGCA
GCCGCGGTAATACGGAGGGTCCAAGCGTTGTCCGGAATCACTGGGCGTAAAGGGTGTGCAGGTGGGGCAGCAAGTCAGAGGTGAAA
GCCCGCGGCTTAACCGCGGAAGTGCCTTTGAAACTGCTGCTCTTGAGTCCCGGAGAGGTTGCCGGAATTCGTGGTGTAGCGGTGAA
ATGCGTAGATATCACGAGGAACACCAGAGGCGAAAGCGGGCAACTGGACGGGTACTGACACTGAGGCACGAAAGCGTGGGGAGCAA
ACAGGATTAGATACCCTGGTAGTCCGCGCTGTAAACGATGAATGCTCGCCGTTGTCTCGTCAAGGGACAGTGGCTAAGCTAACGCG
TTAAGCATTCCGCCTGGGGAGTACGATCGCAAGGTTGAAACTCAAAGGAATTGACGGGGGCCCGCACAAGCGGTGGAGCATGTGGC
TTAATTCGATGCAACGCGAAGAACCTTACCTAGGCTCGAACGCTAGGCGCTCGCTCCTGAAAGGGAGCTTTCCGCAAGGACGCCTA
GCGAGGTACTGCATGGCTGTCGTCAGCTCGTGTCGTGAGATGTTGGGTTAAGTCCCGCAACGAGCGTAACCCCTATTGCTAGTTAC
CATCGGGTAATGCCGGGGACTCTAGTGAGACTGCCTGCGCAAGCAGTGAGGAAGGTGGGGACGACGTCAAGTCATCATGGTCCTTA
CGCCTAGGGCTGCACACGTGCTACATTGGCTGGTACAATGAGCAGCTACACTGCGAGGTGGAGCGAATCTCTGAAAACCAGTCCCA
GTTCGGATTGGAGTCTGCAACTCGACTCCATGAAGCAGGAATCGCTAGTAATCGCGGATCAGCAATGCCGCGGTGAATACGTTCCC
GGGCCTTGTACACACCGCCCGTCAAGCCATGGAAGCTGAGAGCACCCGAAGTCCGTGACCCAACCTTTTGGGAGGGAGCGGCCGAA
GGTGAGCTCAGTGACTGGGGCTAAGTCGTAACAAGGTAGCCGTACCGGAAGGTGCGGCTGGATCACCTCCT
```

### Opening ARB

To launch **ARB**, simply execute the following command in your terminal:

```bash
arb
```

This will open the ARB graphical interface, allowing us to visualize and manipulate 16S rRNA sequences for phylogenetic analysis.


### Importing Sequences into ARB

1. Open **ARB** and load the **LTP database** (`LTP_10_2024.arb`) by selecting **File > Open Database**.
2. Import your **16S rRNA gene sequences** by choosing **File > Import Sequence Data**.
3. Align the imported sequences against the reference database using the **SINA** tool.

### Taxonomic Classification

1. Add the aligned sequence to the LTP phylogenetic tree using the parsimony tool.
2. Assign taxonomy based on the **closest reference sequences**.
3. Select the close relative sequences for phylogenetic tree reconstruction.

### Constructing a Phylogenetic Tree

1. Select the sequences you wish to include in the phylogenetic analysis.
2. Go to **Tree** and **Build tree from sequence data**, and select:
   - **Maximum Likelihood (ML)**
   - **Neighbor-Joining (NJ)**
   - **Maximum Parsimony (MP)**
3. Generate and visualize the **phylogenetic tree** to determine the taxonomic position of your sequences.

## Summary

By the end of this workshop, participants will have a solid understanding of:
- The importance of the **LTP database** in microbial taxonomy.
- The process of aligning, analyzing, and classifying **16S rRNA sequences**.
- How to generate a **phylogenetic tree** and interpret taxonomic relationships.



