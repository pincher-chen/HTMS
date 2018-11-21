# 1.Input files
```
#Four basis files
INCAR POSCAR POTCAR KPOINTS
```
## 1.1.How to get INCAR
A template for generating INCAR
```
#The elementary parameters which control the type of calculations and systems
SYSTEM=FeCo2S4
ISTART=0
ICHARG=2
ENCUT=450 #important
ISMEAR=1
ISPIN=2  #important, you shoud be familar with your materials, magnetic or not.

#the advanced control of calculation methods and convergence conditions
PREC=Normal
EDIFF=1E-05
LREAL=Auto
ALGO=Fast
GGA=PE  #important, be consistent with you pseudopotential.
IBRION=2
NSW=500
EDIFFG=-1E-02
ISIF=2  #important, fixed lattice or not
SYMPREC=1E-8

#the parameter for LDA+U OR GGA+U
LDAU=.TRUE.
LDAUTYPE=2
LDAUL=-1 2 2 
LDAUU=0.00 3.50 0.50 #important, empirical method
LDAUJ=0.00 0.00 0.00  #important, empirical method
LDAUPRINT=2
LMAXMIX=6
```
## 1.2.How to get POSCAR
## 1.3.How to get POTCAR
## 1.4.How to get KPOINTS

# 2.Analysis
## 2.1.DOS
## 2.2.Charge density difference
## 2.3.Band Structure
