### This is an exmple for Black phosphorene 

* To Test the program:

change the workdir variable in following files to your current directory

```
./elc_energy/Mech2D.json
./elc_stress/Mech2D.json
./ssc_stress/Mech2D.json
```
if your current work directory (get it by `pwd` command) is :

/home/zhangsan/mech2d/examples/alpha-P-R

then you set:
"workdir": "/home/zhangsan/mech2d/examples/alpha-P-R/elc_energy"

then you can analysis the mechanics properties by using the following commands:

```
m2d post -a energy --plot
m2d post -a stress --plot
m2d post -a stress -p ssc 
```

or use this help command

```
m2d -h

```
or 

```
m2d init -h
```
* To run the example from new

1. make sure that you have the right configure file "input.yaml"
2. sh run.sh
