# Red Edge Prototypes

This repository is part of my capstone project at the Rochester Institute of Technology. We are modeling the climate of the exo-planet TRAPPIST1-e with the intention of subjecting organisms and microbes to the environment using a climate chamber. We will be using a climate modeling package written in Fortran called [Atmos](https://github.com/VirtualPlanetaryLaboratory/atmos) and a time series GAN model called [TimeGans](https://github.com/jsyoon0823/TimeGAN). Check [Trappist1_parameters.mkd](https://github.com/CryptoTheSuperDog/CapstoneProject/blob/main/Trappist_parameters.mkd) for the data for the PLANET.dat file if using TRAPPIST-1e.

# Packages and Environment
All of the code is going to be written in python but there are specific versions needed. Also there is some fortran code that Atmos must run so a fortran compiler is needed as well. 
* Python(3.7) because tensorflow 1.15.0 is being used in TimeGan and any other version after 3.7 can not install it. Tensorflow has depreciated some functions
* tensorflow 1.15.0
* numpy>=1.17.2
* tqdm>=4.36.1
* argparse>=1.1
* pandas>=0.25.1
* scikit-learn>=0.21.3
* matplotlib>=3.1.1
* Any fortran compiler (I used [gfortran](https://gcc.gnu.org/wiki/GFortranBinaries))

# Run Current code
First make sure all programs are in the same directory. 
Create a template for the planet in the atmos/PHOTOCHEM/INPUTFILES/TEMPLATES. Specificly you want to copy and edit an existing PLANET.dat folder atmos has and change what is needed.
Customize parameters in the main.py file based on the helpful comments
Run and Enjoy!
