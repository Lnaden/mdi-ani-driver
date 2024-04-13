# Molecular Dynamics with TorchANI

This repository contains a prototype implementation of a molecular dynamics simulation using the ANI2x neural network potential. 
The code uses [TorchANI](https://aiqm.github.io/torchani/index.html) to calculate forces, and [LAMMPS](https://www.lammps.org/#gsc.tab=0) to perform the simulation. Communication between the codes is controlled with the [MolSSI Driver Interface](https://molssi-mdi.github.io/MDI_Library/html/index.html) (MDI).

To run this code, you should install Docker and MDIMechanic. You can find instructions for installing Docker [here](https://docs.docker.com/get-docker/).

To install MDI Mechanic, make a Python environment, and do:

```
pip install mdimechanic
```

To run the code, first build in the repository using mdimechanic:

```
mdimechanic build
```

Then, run the code using mdimechanic:

```
mdimechanc run --name ani
```

The output files will be in the `lammps` directory.