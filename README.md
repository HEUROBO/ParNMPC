# ParNMPC Version 1903-1

### New Features in Version 1903-1:
* Primal-dual interior-point method
* Improved user interface
* Better performance
* Line search

## Introduction
Homepage: https://deng-haoyang.github.io/ParNMPC/

**`ParNMPC`** is a MATLAB real-time optimization toolkit for nonlinear model predictive control (NMPC). 
The purpose of **`ParNMPC`** is to provide an easy-to-use environment for NMPC problem formulation, closed-loop simulation, and deployment.

With **`ParNMPC`**, you can define your own NMPC problem in a very easy way and **`ParNMPC`** will automatically generate self-contained C/C++ code for single- or multi-core CPUs. 

**`ParNMPC`** is very fast even with only one core (the computation time is usually in the range of $\mu$s), and a high speedup can be achieved when parallel computing is enabled.

### Highlights
* Symbolic problem representation
* Automatic parallel C/C++ code generation with OpenMP
* Fast rate of convergence (up to be superlinear)
* Highly parallelizable (capable of using at most N cores, N is the # of discretization steps)
* High speedup ratio
* MATLAB & Simulink 

## Installation

1. Clone or download **`ParNMPC`**.
2. Extract the downloaded file.

## Requirements

* MATLAB 2016a or later
* MATLAB Coder
* MATLAB Optimization Toolbox
* MATLAB Parallel Computing Toolbox
* MATLAB Symbolic Math Toolbox
* Simulink Coder
* C/C++ compiler supporting parallel code generation

## Getting Started (MATLAB 2018b)

1. Select the Microsoft Visual C++ 2017 (C) compiler:
``` Matlab
>> mex -setup
```

2. Navigate to the *Quadrotor/* folder.
``` Matlab
>> cd  Quadrotor/
```

3. Open `NMPC_Problem_Formulation.m` and run. 

4. Open `Simu_Simulink_Setup.m` and run. 

5. Open `Simu_Simulink.slx` and run. 


## Citing ParNMPC

Citing the parallel algorithm:

```
@article{deng2019parallel,
  title={A parallel Newton-type method for nonlinear model predictive control},
  author={Deng, Haoyang and Ohtsuka, Toshiyuki},
  journal={Automatica},
  volume={109},
  pages={108560},
  year={2019}}
```
Citing the toolbox (conference version):

```
@inproceedings{deng2018parallel,
  title={A parallel code generation toolkit for nonlinear model predictive control},
  author={Deng, Haoyang and Ohtsuka, Toshiyuki},
  booktitle={Proceedings of the 57th {IEEE} {C}onference on {D}ecision and {C}ontrol},
  pages={4920--4926},
  year={2018},
  address={Miami, USA}}
```

## License

ParNMPC is distributed under the BSD 2-Clause "Simplified" License.
