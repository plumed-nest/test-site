# Fes From Hell potential

This folder contains the scripts to generate a Fes From Hell potential (FFH) used in the ATLAS paper. 

The script that generate the parameters for the potential generate a JSON file that contains all the details for the FFH.
Given that is a JSON format, it is easier to generate the parameters with the script, and then eventually fine tune the potential
by editing directly the JSON file.

If no other parameter than the number of dimension is provided, then the script automatically generate the points for the creating the minima.
The way in which the points are generated is the same as the one used in the ATLAS paper, and is summarized below:

For a 3D system we have 4 points and 4 minima:
 points  
 1  1  1  
 1  1 -1
 1 -1  1
-1  1 -1

with the last minimum connecting the first.

```bash
python3 generate_FFH.py -d 6
```

Generate 7 points and 7 minima

Alternatively, you can generate the parameters starting from a list of points in an txt file

```bash
python3 generate_FFH.py -d 3 -f points.txt 
```

The keyword *sigma* and *exp* are used to set the sigma and exponent parameters in the FFH equation.

After that the FFH JSON file has been generated, it is possible to create an input for PLUMED by converting it through

```bash
python3 convert_FFH_plumed.py -j FFH.json -p plumed_FFH.dat
```

The script generate the plumed and the input file required to perform a langevin simulation with ATLAS. 
A clusters.dat file is also generated to illustrate how the file that ATLAS need containing the GMM should be formatted.
This file may be used to run the calculation, **but it is not guaranteed that the simulation will perform in an optimal way**
This is because we have used the rotation matrix **R** used to generate the potential as proxy for the covariance matrix, and 
we guessed the weight of each cluster as 1/N where N is the number of clusters.

