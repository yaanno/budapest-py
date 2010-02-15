# What

Here I'll show a few -hopefully- useful scripts and utilities for
building Python development environments with ease.

## How

In a few steps I'll build a nice environment management in general and
specific environments to go with different Python versions, packages
or even projects.

## What the hell for? I have bash scripts to do this!

I'm sure you had to develop on different workstations, platforms, versions
and server environments and finally you have a well settled system you don't
want to ruin with experimental software and so on. With a few useful tools 
you can make your life easier without giving up the development mental flow
and the system integrity of yours.

## Basic requirements

* Python (obviously)
* easy_install
* virtualenv
* pip

### Python

On modern systems you'll have at least two Python versions: 2.5 and 2.6,
but older ones are to go as well. NB: I won't cover Windows specific issues,
sorry.

### easy_install

We'll use this to grab the necessary packages for the next steps and
forget it immediately. If you don't have easy_install, download [setuptools](http://pypi.python.org/pypi/setuptools)
from PyPI and install it the normal way with 
    python setup.py install
after unpacking.

### virtualenv

We'll use [virtualenv](http://pypi.python.org/pypi/virtualenv/) for its coolness extensively, so after you went along
with easy_install, do an 
    easy_install virtualenv

### pip

[pip](http://pypi.python.org/pypi/pip/) is a great and nice package management tool that deserve attention from
every Python developer, so lets put it into the site-packages immediately:
    easy_install pip

## Building steps

## Useful links

## Thanks