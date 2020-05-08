## Project Overview

Computational biology involves immense volumes of data in sequences of DNA. A common question about the sequences is, "how similar are two or more sequences?" k-mers are a widespreach tool to answer the question. k-mers are segments of legnth k that are in the larger sequence. Comparing which k-mers are in two different sequences can measure the similarity between sequences.

A way to address the issue of the large number of k-mers that are involved in these comparisons is to use MinHash. This approach creates "sketches" made of subsets of the k-mers in a sequence. The sketches save memory use and compute time.

This project builds on existing work on k-mer sketchers to develop a parallelized, distributed implementation of a k-mer sketcher. Using parallel I/O and k-mer selection prediction, the project focuses on creating an efficient and usable system.

## Research References

Did (https://math.stackexchange.com/users/6179/did). Finding expected number of distinct values selected from a set of integers. Mathematics Stack Exchange. URL:https://math.stackexchange.com/q/72229 (version: 2017-07-20).

Guillaume Marçais, Dan DeBlasio, Prashant Pandey, Carl Kingsford, Locality-sensitive hashing for the edit distance, Bioinformatics, Volume 35, Issue 14, July 2019, Pages i127–i135, [https://doi.org/10.1093/bioinformatics/btz354](https://doi.org/10.1093/bioinformatics/btz354)

Langmead BT and Baker D. Genomic sketching with HyperLogLog [version 1; not peer reviewed]. F1000Research 2019, 8:1866 (slides) [(https://doi.org/10.7490/f1000research.1117605.1)](https://doi.org/10.7490/f1000research.1117605.1)

Rowe, W.P.M. When the levee breaks: a practical guide to sketching algorithms for processing the flood of genomic data. Genome Biol 20, 199 (2019) [doi:10.1186/s13059-019-1809-x](https://doi.org/10.1186/s13059-019-1809-x)

Ondov, B.D., Treangen, T.J., Melsted, P. *et al.* Mash: fast genome and metagenome distance estimation using MinHash. *Genome Biol* 17, 132 (2016) [doi:10.1186/s13059-016-0997-x](https://doi.org/10.1186/s13059-016-0997-x)
