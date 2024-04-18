# This is a readme file to document the installation process

## Installation in python3.9 environment 

The mmaction2 can be installed in a python3.9 env, with 

pip install torch==2.1.0+cu121 -f https://download.pytorch.org/whl/torch_stable.html
pip install torchvision==0.16
mmcv==2.1.0

The installation can generally follow (https://mmaction2.readthedocs.io/en/latest/get_started/installation.html)
There might be hicups when installing chumpy, lower the pip version to 19.0 might help.

## installation in python3.12 environment

pip install torch==2.2.0+cu121 -f https://download.pytorch.org/whl/torch_stable.html
pip install torchvision==0.17
mmcv==2.1.0
note that mmcv needs to be build from source (https://mmcv.readthedocs.io/en/latest/get_started/build.html#)

The 2.1.0 release of mmcv can be downloaded from (https://github.com/open-mmlab/mmcv/releases)

I did notice there was a pip complain saying that setuptools/69.5.1 is not compatible with openxlab/0.0.38 (which needs 60. something), but so far it has not been causing issues

when installing chumpy (for mmpose), there is pip not recognized error. using the following to reinstall pip could help

wget https://bootstrap.pypa.io/get-pip.py
python get-pip.py


