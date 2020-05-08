## Project Overview

Genetic research involves immense volumes of data in sequences of DNA. A common question about the sequences is: how similar are two or more sequences? A widespread approach to answering the question is using k-mers, which are segments of length k that make up the larger sequence. Comparing the sets of k-mers for the sequences can give an estimate of the similarity between the sequences.

This project builds on existing work on k-mer sketchers to develop a parallelized, distributed implementation of a k-mer sketcher. K-mer sketching, as an alternative to the more precise k-mer counting, addresses issues of memory limitations, as it effectively compresses the data, resulting in a compact summary of the data with a lower level of error than sampling offers. This project focuses on creating an efficient and usable system.

## Background Material

[Base k-mer Sketcher - sketch](https://github.com/dnbaker/sketch)

[Mash Paper](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-0997-x)

[Sketch Slides](https://f1000research.com/slides/8-1866)
