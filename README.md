# python_course_2024

# download miniconda
https://conda-forge.org/downloadwget 
´wget https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh´


# install miniconda
`chmod u+x miniforge3-Linux-x86._64.sh
./miniforge3-Linux-x86._64.sh´
## do not activate conda during installation

# source the conda file
source miniforge3/etc/profile.d/conda.sh 

# create alias to source the file (optional but recommended)
open text editor
type alias condaon='source ~/miniforge3/etc/profile.d/conda.sh'
save file as .bashrc in home folder
in terminal execute
chmod u+x .bashrc

# create a conda environment (or core)

when conda is active
type conda create -n name_of_core python==3.12

# activate an environment
when conda is active type
conda activate name_of_core


