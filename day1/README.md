# Day 1
## Retreiving a structure

We will take the skc1 gene from *Streptomyces lividans* coding for a potassium channel protein as a toy exaple. 
First let's look to the [genomic sequence from GenBank.](https://www.ncbi.nlm.nih.gov/nuccore/Z37969)
If you explore the file you will find a cross reference to the Uniprot database. We can use it to reach the entry in the [Uniprot database](https://www.uniprot.org/). 


* What is the name of the protein encoded by skc1 gene.
* Find the structure section, how many structures are available for this protein ?
* Can you check if the entire protein's structure is solved ?


![Pyruvate kinase protein](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7a/Pyruvate_kinase_protein_domains.png/250px-Pyruvate_kinase_protein_domains.png)

We are now going to the [RCSB](https://www.rcsb.org/) web page (The protein databank). Let us use the PDB code [1BL8](https://www.rcsb.org/structure/1BL8) in the search field to access to the structure. 

Click the download file button then select "PDB format" to download the file.


## Exploring the structure in text mode
Identify these different parts in the PDB file. 

##### The header
```
HEADER    MEMBRANE PROTEIN                        23-JUL-98   1BL8              
TITLE     POTASSIUM CHANNEL (KCSA) FROM STREPTOMYCES LIVIDANS                   
COMPND    MOL_ID: 1;                                                            
COMPND   2 MOLECULE: PROTEIN (POTASSIUM CHANNEL PROTEIN);                       
COMPND   3 CHAIN: A, B, C, D;                                                   
COMPND   4 ENGINEERED: YES;                                                     
COMPND   5 MUTATION: YES                                                        
SOURCE    MOL_ID: 1;                                                            
SOURCE   2 ORGANISM_SCIENTIFIC: STREPTOMYCES LIVIDANS;                          
SOURCE   3 ORGANISM_TAXID: 1916;                                                
SOURCE   4 EXPRESSION_SYSTEM: ESCHERICHIA COLI;                                 
SOURCE   5 EXPRESSION_SYSTEM_TAXID: 562;                                        
SOURCE   6 EXPRESSION_SYSTEM_STRAIN: XL-1 BLUE;                                 
SOURCE   7 EXPRESSION_SYSTEM_PLASMID: PQE60;                                    
SOURCE   8 EXPRESSION_SYSTEM_GENE: KCSA   

```


##### Atoms and Hetero atoms


```
ATOM      1  N   ALA A  23      65.191  22.037  48.576  1.00181.62           N  
ATOM      2  CA  ALA A  23      66.434  22.838  48.377  1.00181.62           C  
ATOM      3  C   ALA A  23      66.148  24.075  47.534  1.00181.62           C  
ATOM      4  O   ALA A  23      65.327  24.916  47.902  1.00181.62           O  
ATOM      5  CB  ALA A  23      67.503  21.981  47.702  1.00 74.09           C  

.
.
.
HETATM 2825  K     K A 401      67.868  26.595   9.017  1.00 57.73           K  
HETATM 2826  K     K A 402      70.574  26.590  15.816  1.00 74.76           K  
HETATM 2827  K     K A 403      71.815  26.478  18.867  1.00 75.52           K  
HETATM 2828  O   HOH B 500      69.120  26.480  12.189  1.00 66.21           O
```


##### Connection section 


```
CONECT 2496 2827                                                                
CONECT 2501 2826                                                                
CONECT 2508 2825                                                                
CONECT 2512 2825  
```


* Extract the first chain of the structure in an independant file. 

Verify if the sequence of the chain is the same as the protein in the Uniprot entry. We hace first to convert the data in the PDB file to get the sequence. We can use the [WhatIF server](https://swift.cmbi.umcn.nl/servers/html/soupir.html). We then align the sequence to the Uniprot entry using [EMBOSS needle server](https://www.ebi.ac.uk/Tools/psa/emboss_needle/).


## NMR structures
In the same manner as before download the struture of [Charybdotoxin](https://www.rcsb.org/structure/2crd). 

* What is the Uniprot identifier of the peptide.
*  Try to identify the constructing blocks of the file. 
*  Extract the sequence from the PDB file and compare it to the sequence from the metadada (use ), again using [WhatIF server](https://swift.cmbi.umcn.nl/servers/html/soupir.html) and [EMBOSS needle server](https://www.ebi.ac.uk/Tools/psa/emboss_needle/). 


