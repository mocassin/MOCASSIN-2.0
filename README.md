## MOCASSIN-2.0
[![Build Status](https://travis-ci.org/mocassin/MOCASSIN-2.0.svg?branch=master)](https://travis-ci.org/mocassin/MOCASSIN-2.0)
[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/mocassin/mocassin-2.0)

**MOnte CArlo SimulationS of Ionized Nebulae**, Version 2.0

*3D Monte Carlo Photoionization and Dust Radiative Transfer Code*

Copyright (C) 2005 Barbara Ercolano

### Installation

How to compile:

    make mocassin
    make mocassinWarm
    make mocassinOutput
    make mocassinPlot

What typical packages required to compile mocassin on linux:

    gcc openmpi

or

    intel/mpi

How to clean:

    make clean
     
How to run:

    mpirun -np N ./mocassin

where N is number of processors for parallel computing.

How to run mpirun on a supercomputer:

In the [batches folder](https://github.com/equib/mocassin-models/tree/master/batches) of [mocassin-models](https://github.com/equib/mocassin-models), there are running batch examples for different job scheduling systems. 

To submit a batch file on the Portable Batch System (*PBS*):

     qsub mocassin_run.job

To submit a batch file on the Sun Grid Engine (*SGE*):

     qsub mocassin_run.job

To submit a batch file on the Simple Linux Utility for Resource Management (*SLURM*): 

     sbatch mocassin_run.sh

### References

* Ercolano, B., Barlow, M. J., Storey, P. J., & Liu, X.-W., "MOCASSIN: a fully three-dimensional Monte Carlo photoionization code", [MNRAS, 340, 1136, 2003](http://adsabs.harvard.edu/abs/2003MNRAS.340.1136E)

* Ercolano, B., Barlow, M. J., \& Storey, P. J., "The dusty MOCASSIN: fully self-consistent 3D photoionization and dust radiative transfer models", [MNRAS, 362, 1038, 2005](http://adsabs.harvard.edu/abs/2005MNRAS.362.1038E)
