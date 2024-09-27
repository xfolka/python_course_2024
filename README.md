# python_course_2024

## download miniconda
Browse to

https://conda-forge.org/downloadwget 
or, in a terminal, execute

```wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh```


## Install miniconda
```
chmod u+x miniforge3-Linux-x86._64.sh
./miniforge3-Linux-x86._64.sh
```

**_Do NOT activate conda during installation_**

## Source the conda file
```source miniforge3/etc/profile.d/conda.sh ```

### Create alias to source the file (optional but recommended)
open text editor and type
```alias condaon='source ~/miniforge3/etc/profile.d/conda.sh'```
in an empty file.

save file as .bashrc in home folder.

In terminal execute
```chmod u+x .bashrc```
Open a new terminal and type
```condaon```
this will activate conda an give access to the conda command

## Create a conda environment (or core)

When conda is active, type 
```conda create -n name_of_env python==3.12```
Where ```python==3.12``` means we want a specific version (3.12) of python in this environment
and ```name_of_env``` is the name you want to give your environment.
Use something that allows you to remember what it is used for.

## Activate an environment
when conda is active type
```conda activate name_of_env```

## Installing python modules with Pip

## More information / Documentation
Documentation for conda/Miniforge can be found here:
https://conda-forge.org/docs/user/



