
[![Build Status](https://travis-ci.org/hernanchavezthielemann/GRO2LAM.svg?branch=20jul18)](https://travis-ci.org/hernanchavezthielemann/GRO2LAM)

# GRO2LAM
Gromacs to Lammps simulation converter

## Version:
   GROTOLAM version 1.11 (20 Jul 2018)
   
## Table of contents

<!--ts-->
   * [Version](#version)
   * [Table of contents](#table-of-contents)
   * [Description](#description)
   * [Installation](#installation)
      * [Quantum start](#quantum-start)
      * [Quick start](#quick-start)
      * [Step by step](#step-by-step)
   * [Usage](#usage)
      * [Lammps data file generation](#lammps-data-file-generation)
      * [Lammps input file generation](#lammps-input-file-generation) 
      * [Lammps simulation launching](#lammps-simulation-launching) 
   * [License](#license)
   * [Files](#files)   
   * [Code Datastream Highlights](#code-datastream-highlights)
<!--te-->

## Authors

- Python version:
    Hernan Chavez Thielemann

## Description
This program was designed for easy conversion of solvated structures between 
the GROningen MAchine for Chemical Simulations([Gromacs]) and the 
Large-scale Atomic Molecular Massively Parallel Simulator ([Lammps]). 
It is a python modular routine used to convert 5 [Gromacs] files to 2 [Lammps] format files,
this includes topology, force field coefficients and simulation commands.

## Installation

### Quantum start:

    wget https://raw.githubusercontent.com/hernanchavezthielemann/utils/master/grotolam/G2L_installer && bash G2L_installer
    
### Quick start:

    #!/bin/bash
    wget https://github.com/hernanchavezthielemann/GRO2LAM/archive/20jul18.zip
    unzip 20jul18.zip
    cd GRO2LAM-*
    python setup
    ./run


### Step by step:

Download from:

https://github.com/hernanchavezthielemann/GRO2LAM/archive/20jul18.zip

Unpack, or you can open a terminal and then execute:
    
    ~$ wget https://github.com/hernanchavezthielemann/GRO2LAM/archive/20jul18.zip
    ~$ unzip master.zip
    
Then, make sure that terminal is in the GROTOLAM folder. As example:
    
    user@system:~/Downloads/GRO2LAM-20jul18$
    
Once there, execute the setup file through the terminal as:
    
    ~$ python setup
Then, without changing the folder, execute the run script:
    
    ~$ ./run
After that an intuitive graphical user interface should appear


## Usage

## # GUI
   Follow the secuential menu bar.
   
   <p align="center">
   <img src="https://i.imgur.com/gbI5H7y.gif" title="source: imgur.com" />
   </p>
   
   This will create [Lammps] simulation files with setup parameters inherited from [Gromacs].
    
## # Command line interface
   There is no implementation of comand line interface, more than:
   ```bash
   ~$ python setup -t
   ```
   That creates a not fully useful test GUI.
   
## Licence
   [MIT](./LICENSE)
   
   This work is also licensed under the Creative Commons Attribution 4.0 International License. 
   To view a copy of this license, visit http://creativecommons.org/licenses/by/4.0/ or send a letter to Creative Commons, 
   PO Box 1866, Mountain View, CA 94042, USA.

## Citation
   The publication associated with this code is found here:



[Lammps]: http://lammps.sandia.gov/
[Gromacs]: http://www.gromacs.org/
