---
title: Virtualenv on Mac with Conda (Anaconda)
date: "2015-05-25"
description: 
tags: 
- Anaconda, conda
---

Pressing the Launch button on Anaconda Navigator results in appearing of a Mac terminal and long hanging.... The Jupyter notebook doesn't start. 

It starts from an iTerm, with a command

jupyter notebook

- but sometimes it defaults to Python2.7, and then it's a message 

-bash: command jupyter is not found

- and then I have to specify a path to anaconda3:

```
export PATH=~/anaconda3/bin:$PATH
conda --version
which jupyter
which python
```

That feeling when, after some head-banging, a snippet of advise is found on internet... Like a ray of sunshine...

Frustrated (for the Nth time) with Bash rejecting some commands on Mac, `-bash: command XXX doesn't exist`, this time, the virtualenv command.... And the suggestions on the web always revolve arouth $PATH, .bash-profile, .bashrc... which doesn't seem to make any difference...

So thankful to have found this tiny answer (4th on this page) that if Anaconda package manager is installed , it basically takes over the virtual environment management. 

[Error “virtualenv : command not found” but install location is in PYTHONPATH](https://stackoverflow.com/questions/39964635/error-virtualenv-command-not-found-but-install-location-is-in-pythonpath?noredirect=1&lq=1)

[conda create ](../assets/conda_virtualenv.png)