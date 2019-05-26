---
title: Today I learned
date: "2015-05-25"
description: 
tags: 
- today I learned
---
### 05-25-2019: the mess with virtualenv and conda (Anaconda, Miniconda) is resolved.

If you have Anaconda installed, then the usual virtualenv activation from the command line doesn't work. It is now done with conda. 

```conda -v

conda update conda

conda search "^python$"

conda create -n yourenvname python=x.x anaconda```

Press y to proceed. This will install the Python version and all the associated anaconda packaged libraries at `path_to_your_anaconda_location/anaconda3/envs/yourenvname`.


```conda info -e

source activate yourenvname

$ source activate venv
(venv) $

source deactivate

conda remove -n yourenvname -all``

[Getting started with Conda](https://conda.io/projects/conda/en/latest/user-guide/getting-started.html#)

[Create virtual environments for python with conda](https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/20/conda/)
