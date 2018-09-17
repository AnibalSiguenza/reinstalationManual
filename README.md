# Reinstalation Manual
Guide to install all the tools I need

## MPI

### MPICH

```
sudo apt-get install mpich
```

### Open MPI
```
sudo apt-get install openmpi-common
sudo apt-get install libcr-dev libopenmpi-dev openmpi-bin openmpi-doc
```
## Paraview

```
sudo apt-get install paraview  
```

Note: this also installs openMPI which can unset the proper behavior of mpi because it changes the binary link from mpirun. You need to make sure that the mpirun and mpirc++ point both to the same distribution.

1. check the links on the bin
```
cd /usr/bin && ll mpi*
cd /etc/alternatives && ll mpi*
```

