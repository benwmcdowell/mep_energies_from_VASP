Plots the energies for each image in a minimum energy pathway (MEP) calculation with VASP. Plotting the initial and final energy profiles is useful for gauging convergence progress during an optimization.

Run this script in the home directory, containing the INCAR file and each image sub-directory. The OUTCARs corresponding to the converged run of the initial and final mep images must be copied into the directories named 00/ and images+1/. By default, the script is executed in the current directory, but other locations can be specified with -i,--input.

The reaction coordinate is normalized so that the image in directory 00/ is at 0.0 and the image in directory images+1/ is at 1.0. Energies are plotted relative to the minimum energy in the MEP series.

Example of intended usage: python mep_energy or python mep_energy -i my_mep_directory
