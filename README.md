# Jupyter Lab Sandbox
Quickstart Python JupyterLab environment

## Pre-requsites
| Command | Output |
| --- | --- |
| conda --version	| conda 4.5.12 |
| gcc --version	| gcc (Homebrew GCC 8.2.0) 8.2.0 |
| pip --version	| pip 18.1 from /anaconda3/envs/jupyterlab/lib/python3.7/site-| | packages/pip (python 3.7) |
| python --version | Python 3.7.1 |
| uname -a	| Darwin <hostname> 17.7.0 Darwin Kernel Version 17.7.0: Thu Jun 21 22:53:14 PDT 2018; root:xnu-4570.71.2~1/RELEASE_X86_64 x86_64 |


## Install
```
cd ~
conda create --name jupyterlab --yes jupyterlab
conda activate jupyterlab

jupyter labextension install @jupyterlab/git
pip install jupyterlab-git
jupyter serverextension enable --py jupyterlab_git
```
## Requirements
```
appnope==0.1.0
backcall==0.1.0
bleach==3.0.2
certifi==2018.11.29
decorator==4.3.0
entrypoints==0.2.3
ipykernel==5.1.0
ipython==7.2.0
ipython-genutils==0.2.0
jedi==0.13.2
Jinja2==2.10
jsonschema==2.6.0
jupyter-client==5.2.4
jupyter-core==4.4.0
jupyterlab==0.35.3
jupyterlab-git==0.5.0
jupyterlab-server==0.2.0
MarkupSafe==1.1.0
mistune==0.8.4
nbconvert==5.3.1
nbformat==4.4.0
notebook==5.7.4
pandocfilters==1.4.2
parso==0.3.1
pexpect==4.6.0
pickleshare==0.7.5
prometheus-client==0.5.0
prompt-toolkit==2.0.7
psutil==5.4.8
ptyprocess==0.6.0
Pygments==2.3.1
python-dateutil==2.7.5
pyzmq==17.1.2
Send2Trash==1.5.0
six==1.12.0
terminado==0.8.1
testpath==0.4.2
tornado==5.1.1
traitlets==4.3.2
wcwidth==0.1.7
webencodings==0.5.1
```
## Start
```
conda activate jupyterlab
cd ~
jupyter lab
```
## Uninstall
```
conda deactivate jupyterlab
conda env remove --name jupyterlab
```