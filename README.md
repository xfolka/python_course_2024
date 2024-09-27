# python_course_2024

## download miniconda
https://conda-forge.org/downloadwget 
´wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh´


## install miniconda
```
chmod u+x miniforge3-Linux-x86._64.sh
./miniforge3-Linux-x86._64.sh
```

### do not activate conda during installation

## source the conda file
```source miniforge3/etc/profile.d/conda.sh ```

## create alias to source the file (optional but recommended)
open text editor and type 
```alias condaon='source ~/miniforge3/etc/profile.d/conda.sh'```
in an empty file.
save file as .bashrc in home folder.

In terminal execute
```chmod u+x .bashrc```
Open a new terminal and type
```condaon```
this will activate conda an give access to the conda command

## create a conda environment (or core)

When conda is active, type 
```conda create -n name_of_env python==3.12```
Where ```python==3.12``` means we want a specific version (3.12) of python in this environment
and ```name_of_env``` is the name you want to give your environment.
Use something that allows you to remember what it is used for.

## activate an environment
when conda is active type
```conda activate name_of_env```

## installing python modules with Pip



