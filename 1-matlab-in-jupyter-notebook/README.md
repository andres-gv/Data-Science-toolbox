# 1. Work in Matlab from a Jupyter Notebook
python3.6 -m venv ~/python-venvs/matlab-jupyter-py36
source ~/python-venvs/matlab-jupyter-py36/bin/activate
pip install -U pip
pip install jupyterlab pandas

pip install matlab_kernel
python -m matlab_kernel install --user
jupyter kernelspec list

cd /opt/matlab2018a/extern/engines/python/
python setup.py install
jupyter notebook
