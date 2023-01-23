# PyEED-jupyternotebook
Jupyter notebook datamodel\
This data model consists of a pipeline work to be used for biological analysis uses, as the data gathering step is over all of the data will be stored in a database of your creation, later the database can be expended or the data can be used for further analysis.\

The pipe line starts with all of the required installations and packages.\

1.Perform a protein-to-protein BLAST search using a relevant protein fasta file, then record the results in an XML file. All related sequences and accession numbers will be saved inside the xml file.\
2.Each protein's accession number can be used to find the organism name and taxonomy id, later to be inserted into the database.
3.constructing an HMM (Hidden Markov Model) using the protein superfamily that shares the query sequence. Run a multiple sequence alignment on the best five to ten structurally known proteins, then use the HMM Python package's MSA function to produce a consensus HMM.\
4.For the purpose of creating a numbering scheme, compare the relevant sequence to the HMM,choose the finest corresponding sequence that suits your demands. The numbering system will be constructed in sequential order and to assist the user in calculating their own amino acid count, which may then be used, for example, to label specific sequence segments from experimental laboratory work.\
5.For each PDB id, a database of known annotations will be downloaded. You can use this database to compare your own annotation to one that already exists.\
6.In order to extract the DNA nucleotide sequences from the NCBI database, you must first perform a protein to nucleotide tBLASTn search from a relevant protein fasta file and store the tBLASTn results in an XML file.\
7.NCBI DNA ids can be derived from the tBLASTn results that are recorded in the XML file; from these accession numbers, related DNA sequences for each amino acid sequence and corelated DNA NCBI database IDs for each PDB ID can then be found.
