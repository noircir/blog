---
title: Create virtual environments for python with conda
date: "2015-05-25"
description: 
tags: 
- Anaconda, conda, virtual, environmentm, venv
---

conda -v

conda update conda

This one is important!!

conda search "^python$"

conda create -n yourenvname python=x.x anaconda

Press y to proceed. This will install the Python version and all the associated anaconda packaged libraries at “path_to_your_anaconda_location/anaconda3/envs/yourenvname”


conda info -e

source activate yourenvname

$ source activate venv
(venv) $


source deactivate

conda remove -n yourenvname -all



[Getting started with Conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html#)

[Create virtual environments for python with conda](https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/20/conda/)
