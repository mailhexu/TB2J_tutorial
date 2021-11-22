#### The example of how to compute the isotropic/anisotropic exchange, and DMI with TB2J-Siesta interface.

The CrI3 monolayer is the example structure. 

- For doing this calculation, three structures with the original structure roated from z to x, y, and z are required.   The files used for the example of running TB2J_rotate.py to get the three structures are in the rotate_structure directory. Run the command in rotate.sh to get the rotated structures.
- For each of  the generated structures, DFT calculation with Siesta, and the TB2J calculation are performed. The files are done in the DFT directory.  The Siesta output of the Hamiltonian and overlap matrices are in the siesta.nc files in case you just want to try with TB2J.  In each of the directory, run the command in get_J.sh to get the TB2J_results.
- The three results need to be merged. Run the command in merge.sh in the DFT directory to get the merged results in the DFT/TB2J_results directory.
- The reference result is in the TB2J_results directory.
