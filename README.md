## Project Overview

Computational biology involves immense volumes of data in sequences of DNA. A common question about the sequences is, "how similar are two or more sequences?" k-mers are a widespreach tool to answer the question. k-mers are segments of legnth k that are in the larger sequence. Comparing which k-mers are in two different sequences can measure the similarity between sequences.

A way to address the issue of the large number of k-mers that are involved in these comparisons is to use MinHash. This approach creates "sketches" made of subsets of the k-mers in a sequence. The sketches save memory use and compute time.

This project builds on existing work on k-mer sketchers to develop a parallelized, distributed implementation of a k-mer sketcher. Using parallel I/O and k-mer selection prediction, the project focuses on creating an efficient and usable system.

## Background Material

[Base k-mer Sketcher - sketch](https://github.com/dnbaker/sketch)

[Mash Paper](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0997-x)

[Sketch Slides](https://f1000research.com/slides/8-1866)
