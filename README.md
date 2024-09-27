
## Download miniconda
Browse to

https://conda-forge.org/download
or, in a terminal, execute

```wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh```


## Install miniconda
Locate the file on your computer and execute the following in a terminal.

```
chmod u+x miniforge3-Linux-x86._64.sh
./miniforge3-Linux-x86._64.sh
```
OBS! On band the file should be directly in your home directory. It is not there move it there using for example a filemanager or the mv command.

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
Use a name that allows you to remember what it is used for.

## Activate an environment
when conda is active type
```conda activate name_of_env```

Now your environment is active and the packages installed (and only those) are available to you.


## Installing python modules in your environment with Pip
To install python modules we can use a program called ```pip``` like this:
```pip install module``` or ```pip install module==x.y.z``` to install a specific version. I.e.
```
pip install numpy==2.0.0
```
If version is not specified, the latest version available will be installed

## Sharing and reusing environments
Conda allows you to export your environment to share it with others as well as allowing yout to install environments that are shared with you.
To export one of your environments, activate the environment and type:
```conda env export | > environment.yml```
This will store the needed data in the file ```environment.yml```

In order to create an environment from a file you type, in a terminal:
```conda env create -f environment.yml``` 
This will create an environment as specified in the file ```environment.yml```.

Optional: download this environment file to your computer and try to recreate the environment:
https://github.com/xfolka/python_course_2024/blob/main/environment.yml


## More information / Documentation
Documentation for conda/Miniforge can be found here:
https://conda-forge.org/docs/user/



