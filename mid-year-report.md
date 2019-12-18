# Progress Report

View the project at [github.com/kodingkoning/sketch](https://github.com/kodingkoning/sketch). This repo is private, so please send an email to koningelizabeth@gmail.com to request access.

## 1. Project vision and overview
Genetic research involves immense volumes of data in sequences of DNA. A common question about the sequences is: how similar are two or more sequences? A widespread approach to answering the question is using k-mers, which are segments of length k that make up the larger sequence. Comparing the sets of k-mers for the sequences can give an estimate of the similarity between the sequences.

This project builds on existing work on k-mer sketchers to develop a parallelized, distributed implementation of a k-mer sketcher. K-mer sketching, as an alternative to the more precise k-mer counting, addresses issues of memory limitations, as it effectively compresses the data, resulting in a compact summary of the data with a lower level of error than sampling offers. This project focuses on creating an efficient and usable system.

## 2. Background, including research review
There are currently many sequential k-mer sketches that have been developed.

Three existing softwares are:

1. [sketch](https://github.com/dnbaker/sketch)
2. [Mash](https://github.com/marbl/Mash)
3. [OMH](https://github.com/Kingsford-Group/omhismb2019)

## 3. System design, implementation and testing

This project is built off of [sketch](https://github.com/dnbaker/sketch). Of the three existing softwares we evaluated for the project, it is by far the easiest to install and modify.

We decided not to use OMH as the project's base because of 1) challenges with understanding the API and 2) the number of languages used in the project. In order to modify a software for the distributed version, it is necessary to have it in C or C++.

Mash's API was very clear, and it was written entirely in C++. However, its depencies make it difficult to build from source. It also saves results to files between creating a sketch and calculating the distance between two sketches. We anticipate that this would be inefficient in terms of time.

We will be using [BCL](https://github.com/berkeley-container-library/bcl) (Berkely Container Library) ror the distributed data structures.

The next step of the project is profiling the sequential version of sketch.

## 4. Results and discussion

## 5. Conclusions
Conclusions will be made in the spring semester.

## 6. Future work
The future work of the project involves continuing work towards the major goals of the project. Work will be resumed in February.

## 7. Acknowledgements
This project is advised by Dr. Joel Adams at Calvin University, as well as Dr. Aydin Buluc and Dr. Kathy Yelick at UC Berkeley.

Thank you also to PhD students Giulia Guidi and Ben Brock for their consistent support throughout the project.

Development for this project has been on Cori at LBNL.

## 8. References

Guillaume Marçais, Dan DeBlasio, Prashant Pandey, Carl Kingsford, Locality-sensitive hashing for the edit distance, Bioinformatics, Volume 35, Issue 14, July 2019, Pages i127–i135, [https://doi.org/10.1093/bioinformatics/btz354](https://doi.org/10.1093/bioinformatics/btz354)

 Langmead BT and Baker D. Genomic sketching with HyperLogLog [version 1; not peer reviewed]. F1000Research 2019, 8:1866 (slides) [(https://doi.org/10.7490/f1000research.1117605.1)](https://doi.org/10.7490/f1000research.1117605.1)

Rowe, W.P.M. When the levee breaks: a practical guide to sketching algorithms for processing the flood of genomic data. Genome Biol 20, 199 (2019) [doi:10.1186/s13059-019-1809-x](https://doi.org/10.1186/s13059-019-1809-x)

Ondov, B.D., Treangen, T.J., Melsted, P. *et al.* Mash: fast genome and metagenome distance estimation using MinHash. *Genome Biol* 17, 132 (2016) [doi:10.1186/s13059-016-0997-x](https://doi.org/10.1186/s13059-016-0997-x)

