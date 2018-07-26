# *In silico* mutagenesis

*In silico* mutagenesis imply the modification of the structure of a reference protein. This process might introduce some non desirable contacts and atomic clashes. The structure has to be cleaned before any further analysis. 
We are going in this practical to alternate between PyMOL and Chimera. 

1- Open a structure of a protein in PyMOL.
2- Make the mutagenesis.
3- Save the modified structure. 
4- Open the modified structure in Chimera.
5- Make the energy minimization.
6- save the updated structure. 

### Case 1
Open the structure of the KCSA channel from last day. Then mutate the residue G77 of one of the chains with a Trp using the "mutagenesis" option under the wizard menu. Select the best rotameric state and proceed to saving the new structure under the name `KCSA_W77.pdb`.
Run chimera using Ubuntu dock or by typing in the command line:

	$ chimera 

* First open the structure of the mutant and use `Actions > Atoms/Bonds > Show` to show the bonds of the protein. 

* Go to the menu `Tools > structure editing > energy minimization` 
* Adjust the SD and CG steps to 0. 
* Follow the setting of the system and finally hit mninimize. 
* Go to Favorites and open the reply log. Notice the energy value. 
* Before we proceed, select the backbone of the protein: ` Select > Structure >Backbone > minimal`
* Make aother miniminization, this time using 50 steps for SD and 10 Steps for CG. Do not forget to adjust the `fixed atoms` to `selected`.
* Hit minimize and monitor the progree in the log window.
* Now do the same minimization while lifting the backbone constraints. 
* Notice the final energy. Why is it so different from the initial state. 
* Save the minimized structure under the name `KCSA_W77_r.pdb`.
* Open the WT and the refined structure and fit them together. Notice the RMSD value.

### Case 2 

We will now use the same structure of KCSA to mutate the residue N58 to Arg. This will help you to practice the rotamer selection. 

# Exploring the protein complexes

We are going to use pymol to explore the structures of complexes. 

### Case1 : Protein-Ptotein complex 

* Download the structure of `2A9H` from the [protein data bank](www.rcsb.org).
* Open the structure in pymol.
* Define the lif=gand and the receptor and color them differently.
* Define the interface residues on earch of the interaction partners: this will create two objects receptor and ligand. 

```
	select receptor, chain A+B+C+D 
    select ligand, chain E

```
* Use the PyMOL tools to identify polar bonds between the receptor and the ligand. What are probably the most important ones. 
* Could you detect a salt bridge between the pertners. 
* Using the sphere representation, try to identify some key VDW interactions. 
* Query the PDB code to the [Anchor]( http://structure.pitt.edu/anchor) database, does your choice fit with the described data ?

Finally reinitialize pymol, open the same complex again and use the [InterfaceResidues plugin](https://pymolwiki.org/index.php/InterfaceResidues) to extract the residue interface.

### Case2: Protein ligand complex 

* What is the complex described in the entry 3RFM. 
* Use the [Protein-Ligand Interaction Profiler](https://projects.biotec.tu-dresden.de/plip-web/plip/index) to identify the polar bonds between the ligand and the receptor. 
* Open the structure in PyMOL and adjust the view to zoom on the ligand. 
* Extract the ligand's struture to another object and use the surface representation of the protein. 
* What are the residues forming the interaction pocket. 

