# 1. Work in Matlab from a Jupyter Notebook


## Configuration to use Matlab from a Jupyter Notebook

### 1 Create a virtualenv in Python version 3.5 or 3.6
python3.6 -m venv ~/python-venvs/matlab-jupyte

source ~/python-venvs/matlab-jupyter/bin/activate

pip install -U pip

pip install jupyterlab pandas

### 2 Install Matlab API engine for Python
pip install matlab_kernel

python -m matlab_kernel install --user

jupyter kernelspec list


cd /opt/matlab2018a/extern/engines/python/

python setup.py install

### 3 Launch the Jupyter Notebook
jupyter notebook


