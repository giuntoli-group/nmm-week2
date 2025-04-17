# Tutorial 2
For this and following tutorials: some relevant scripts will be in these repositories, but a more complete version can also be found in the Habrok /scratch/hb-nanoscale folder.

The topic of this session will be to optimize the lattice parameters and calculate the electronic properties of bulk materials. You will need to use XCrysDen or the online tool that you tried last week to visualize your structures. 

## Assignment 1

We will start with the DFT calculation of bulk Si. This exercise will consist of the lattice constant optimization and the calculations of the density of states (DOS). Last week, you run the file 'Si.scf.in', and you got familiar with the input parameters and output files. Now, we will continue with the same input file and will set up the calculations to optimize the lattice constant of Si. To this aim, input files with different lattice constants should be prepared. If you are familiar with bash or python scripting, you can easily automatize the file preparation and running. Otherwise, create four empty directories called ‘Si_<lattice_constant>’ using the following set of lattice constants {9.8, 10.0, 10.4, 10.6}. Note that the values in parentheses are expressed in atomic units in accordance with the requirements of QE. Convert them to angstrom (for yourself) to make sure that you know what you are doing. 

Copy the file ‘Si.scf.in’, the pseudopotential file, and the submission script to each directory. Open each of these files using an editor and change the value of the parameter celldm(1) to a corresponding value of lattice constant. Run the job script in each directory.

Once all four calculations are finished, first control that they terminated correctly and then type 
grep ‘!    total energy’ Si.scf.out to check the values of total energy for each lattice constant. Write these values to a file, including the one calculated initially with the lattice constant of 10.26 a.u. 

Use your favorite tool (for example, python, Gnuplot, or if you really want to, MS Excel) to plot the lattice constant vs the total energy curve. Write down the value of the lattice constant for which you see the minimum. Does the optimized lattice constant agree with the experimental value? Compare with the literature. 

## Assignment 2



### Instructions

1a. XXX
