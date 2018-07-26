## Case 1: 
Download the structure of Lamin A [(PDB code:1IFR)](https://raw.githubusercontent.com/hothman/ASBMA_course/master/day3/cases/case1/1ifr_clean.pdb). Mutate the residue R527 by an Asn. Choose the right rotamer and refine with chimera using a tw stages of energy minimization. 

What can be the consequence of this mutation ? 
Use the [SDM](http://marid.bioc.cam.ac.uk/sdm2/) to help you in the analysis. 

![LamA](https://raw.githubusercontent.com/hothman/ASBMA_course/master/day3/figures/mut1.png)

## Case 2
Bacteriorhodopsin is a protein used by Archaea acting as a proton pump to produce chemical energy (ATP). 
Download only the chain B of Bacteriorhodopsin using PyMOL `(fetch 1S51_B)`.  Clean the structure and mutate residue P91 to Gly. Choose the right rotamer and refine with chimera using a tw stages of energy minimization. 
Can you predict the impact of the mutation. 

![Rhod](https://github.com/hothman/ASBMA_course/blob/master/day3/figures/rhod.png?raw=true)

## Case 3 
MMP-2 is an extracellular matrix implicated mainly in collagenolysis. Download the structure of the [catalytic domain 3AYU](https://raw.githubusercontent.com/hothman/ASBMA_course/master/day3/cases/case3/3ayu.pdb). Mutate His 124 with Arg. Choose the best rotamer. Pull you interpretations, this time without refining the structure.
![MMP2](https://github.com/hothman/ASBMA_course/blob/master/day3/figures/mmp2.png?raw=true)


## Case 4
UNC119 is involved in synaptic functions in photoreceptor cells. Download the structure of [3RBQ (CHain C only)](https://raw.githubusercontent.com/hothman/ASBMA_course/master/day3/cases/case4/3rbq.pdb). Again, we are not going to refine the structure prior to the analysis.
![UNC119](https://github.com/hothman/ASBMA_course/blob/master/day3/figures/unc119.png?raw=true)


## Case 5 
Glucocorticoid receptor is a transcription factor which binds to a specific
DNA sequence.
* Download the [structure 3G6P](https://raw.githubusercontent.com/hothman/ASBMA_course/master/day3/cases/case5/3g6p.pdb).
* Create three objects in pymol: DNA, WT and Mut.
* Mutate the Arg 496 tu Asp on both chains for the object Mut.
* Refine the structure and generate the electrostatic map.

![CPLX](https://github.com/hothman/ASBMA_course/blob/master/day3/figures/cplx.png?raw=true)
