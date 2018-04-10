# Repository of computed data 


## Summary 
This repository contains the relevant surface structures computed in the published paper Particle Morphology and Lithium Segregation to Surfaces of the Li<sub>7</sub>La<sub>3</sub>Zr<sub>2</sub>O<sub>12</sub> Solid Electrolyte, P. Canepa *et al.*, *Chem. Mater.* (2018) DOI:

### Only the most stable orderings are archived in this repository.

Two type of surface models are available per each distinct chemical termination: 

* Stoichiometric 
* Off-stoichiometric or nonstoichiometric 

Finally, for certain surface models the effect of Li converage is also explored. 

Additional surface structures (orderings) are available upon request. 
All the structures have been carefully optimized utilizing the [Vienna *Ab initio* Simulation Package](http://www.vasp.at), and the following INCAR file based on the MaterialsProject standards defined via [pymatgen](http://pymatgen.org).  

```
EDIFF  = 1e-06
EDIFFG = -0.01
ENCUT  = 520
ALGO   = Fast
AMIN   = 0.01
AMIX   = 0.2
BMIX   = 0.001
IBRION = 2
ICHARG = 1
ISIF   = 2
ISMEAR = 0
ISPIN  = 1
LORBIT = 11
LPLANE = True
LREAL  = Auto
LWAVE  = False
NELM   = 100
NELMIN = 6
NPAR   = 12
NSW    = 99
PREC   = Accurate
SIGMA  = 0.05
SYMPREC= 1e-8
```
The *k*-point integration mesh was based on the attached KPOINT file. Gamma centering was invoked whenever needed. 

```
Automatic mesh
0
M
2 2 1
```
The PAW potentials used were: 

```
Li: PAW_PBE Li_sv 23Jan2001, 1s2s2p
La: PAW_PBE La 06Sep2000, [core=Kr4d]
Zr: PAW_PBE Zr_sv 07Sep2000, 4s4p5s4d
O:  PAW_PBE O 08Apr2002, s2p4
```