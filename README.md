# PyEED-jupyternotebook
Jupyter notebook datamodel 
This data model consists of a pipeline work to be used for biological analysis uses, as the data gathering step is over all of the data will be stored
in a database of your creation, later the database can be expeded or the data can be used for further analysis.

The pipe line starts with all of the required installations and packages.

1.A protein to protein BLAST search from a protein fasta file of interest and store the BLAST results as an XML file.
2.Extracting the taxonomy id and the organism for each of the resulting BLAST sequences.
3.Creating a HMM(Hidden Markov Model) from the super family of proteins which are related to the query sequence, doing so we take the 5-10 best structurally known proteins and to a multiple sequence alignment, from which we achieve our HMM. We compare the query sequence to the HMM, by which we can create a numbering scheme which later can be used for annotation.
4.A protein to nucleotide tBLASTn search from a protein fasta file of interest and store the tBLASTn results as an XML file, run the accession numbers of the DNAs which were found to extract the DNA nucleotide sequences from the NCBI data base.
