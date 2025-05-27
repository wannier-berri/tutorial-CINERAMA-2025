[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/wannier-berri/tutorial-TMS2023/HEAD)

# Tutorial for CINERAMA conference 2025 (UNDER CONSTRUCTION!!!)

# Overview

The tutorial teaches two things:

1. How to construct Wannier functions
2. How to calculate Brilluin zone integrals (both from tight-binding/kp models and Wannier Functions)

We will use the code [WannierBerri](https://wannier-berri.org/). This code was primarily developed for ab-initio calculations of Berry curvatures and similar quantities (see [paper](https://www.nature.com/articles/s41524-021-00498-5) ) 
also can be equally used for **k.p** or **tight-binding** models. Recently, also construction of Symmetry-adapted Wannier functions is implemented in WB

The tutorials will be provided as [Jupyter](https://jupyter.org/) notebooks  and will de uploaded to this repository 
shortly before the session. So far the students are asked only to prepare their computers 

# Installation

## Briefly: 

TODO : check dependencies

Please install Jupyter Notebook, WanierBerri and also pythtb

```
pip install  --upgrade  pythtb jupyterlab matplotlib wannierberri[all]
```

also, for visualisation of Wannier functions, you may download `VESTA <https://jp-minerals.org/vesta/en/download.html>`_ or `XCRYSDEN <http://www.xcrysden.org/>`_. (or nay other code that accepts xsf files)

## In more words:

First, tutrial is using `python` language. Therefore, please install it on your computer (if not installed yet) 

If you are using Anaconda, please create a new environment with python 3.12


For the tutorial, you will need the following :

1. a portable computer. (Any operation system, it may also be a tablet, it you know how to run python on it).
2. Python interpreter (recommended 3.12, but 3.10, 3.11 and 3.13 shgould also work). python 3.9 is not supported anypore
3. latest versions of wannierberri and irrep (with all their dependencies) and pythtb.
4. jupyter notebook editor (jupyterLab).
O.tionally:.
5. your favourite IDE (Pycharm, VScode, vim,  ...).
6. create a separate virtual environment for the tutorial. It is most conveniently done with anaconda   https://www.anaconda.com/


You may consider the [Anaconda](https://www.anaconda.com/) distribution, but the python which comes with your OS should also be fine. 


You can install everything (after installing anaconda) with the following commands):

``` bash
conda create -n wbvenv python=3.12
conda activate wbvenv
pip install --upgrade wannierberri[all] pythtb jupyterlab
```

After that you may check the installation via by running a few lines:

``` python
import wannierberri as wb
import irrep
import pythtb
print (f"pythtb : {pythtb.__version__}")
print (f"wannierberri : {wb.__version__}")
print (f"irrep : {irrep.__version__}")
parallel = wb.Parallel(num_cpus=4)
parallel.shutdown()
```

 

# If you have problems 

* open an Issue in this repository (you need to login to GitHub for that)
* look through issues in main [repository](https://github.com/wannier-berri/wannier-berri/issues)
* try to find me at the conference (I will be around) 


Looking forward to seeing you at the tutorial!

Stepan Tsirkin
