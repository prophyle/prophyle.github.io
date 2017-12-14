# ProPhyle

## About

ProPhyle is a *k*-mer based metagenomic classifier using Burrows-Wheeler Transform.
Its indexing strategy relies on a bottom-up propagation of *k*-mers in the tree,
assembling contigs at each node, and matching using a standard full-text search using BWT-index.
The analysis of shared *k*-mers between NGS reads and the genomes in the index determines
which nodes are the best candidates for their classification.
More information about the indexing scheme
can be found in our [poster](http://brinda.cz/publications/2017_prophyle_hitseq.pdf).

## Installation

1. Install [Miniconda](https://conda.io/miniconda.html)
2. Add [Bioconda](https://bioconda.github.io/) channels
   ```
   conda config --add channels defaults
   conda config --add channels conda-forge
   conda config --add channels bioconda
   ```
3. Install ProPhyle
   ```
   conda install prophyle
   ```
