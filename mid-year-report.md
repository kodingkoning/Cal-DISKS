## 1. Project vision and overview
Genetic research involves immense volumes of data in sequences of DNA. A common question about the sequences is: how similar are two or more sequences? A widespread approach to answering the question is using k-mers, which are segments of length k that make up the larger sequence. Comparing the sets of k-mers for the sequences can give an estimate of the similarity between the sequences.

This project builds on existing work on k-mer sketchers to develop a parallelized, distributed implementation of a k-mer sketcher. K-mer sketching, as an alternative to the more precise k-mer counting, addresses issues of memory limitations, as it effectively compresses the data, resulting in a compact summary of the data with a lower level of error than sampling offers. This project focuses on creating an efficient and usable system.

## 2. Background, including research review
There are currently many sequential k-mer sketches that have been developed.

Three softwares include:

1. [sketch](https://github.com/dnbaker/sketch)
2. [Mash](https://github.com/marbl/Mash)
3. [OMH](https://github.com/Kingsford-Group/omhismb2019)


## 3. System design, implementation and testing

This project is built off of [sketch](https://github.com/dnbaker/sketch). Of the three, it is by far the easiest to install. Unlike OMH, it has the benefit of being written entirely in C++. Unlike Mash, it was very straightforward to build. Mash has many dependencies.

We decided not to use Mas as the project's base because of the difficulties we had in installing the software from source.



## 4. Results and discussion


## 5. Conclusions
Conclusions will be made in the spring semester.

## 6. Future work
The future work of the project involves continuing work towards the major goals of the project. Work will be resumed in February.

## 7. Acknowledgements
This project is advised by Dr. Joel Adams at Calvin University, as well as Dr. Aydin Buluc and Dr. Kathy Yelick at UC Berkeley.

Thank you also to PhD students Giulia Guidi and Ben Brock for their consistent support throughout the project.

Development for this project has been on Cori and LBNL.

## 8. References

Ondov, B.D., Treangen, T.J., Melsted, P. *et al.* Mash: fast genome and metagenome distance estimation using MinHash. *Genome Biol* 17, 132 (2016) doi:[10.1186/s13059-016-0997-x](https://doi.org/10.1186/s13059-016-0997-x)

