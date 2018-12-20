
## Pre-requsites
conda --version	conda 4.5.12
gcc --version	gcc (Homebrew GCC 8.2.0) 8.2.0
pip --version	pip 18.1 from /anaconda3/envs/jupyterlab/lib/python3.7/site-packages/pip (python 3.7)
python --version	Python 3.7.1
uname -a	Darwin <hostname> 17.7.0 Darwin Kernel Version 17.7.0: Thu Jun 21 22:53:14 PDT 2018; root:xnu-4570.71.2~1/RELEASE_X86_64 x86_64


## Install
cd ~
conda create --name jupyterlab --yes jupyterlab
conda activate jupyterlab

jupyter labextension install @jupyterlab/git
pip install jupyterlab-git
jupyter serverextension enable --py jupyterlab_git


## Uninstall
conda deactivate jupyterlab
conda env remove --name jupyterlab
