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

### pip

[pip](http://pypi.python.org/pypi/pip/) is a great and nice package management tool that deserve attention from
every Python developer, so lets put it into the site-packages immediately:
    easy_install pip

### virtualenv

We'll use [virtualenv](http://pypi.python.org/pypi/virtualenv/) for its coolness extensively, so after you went along
with easy_install, do an 
    pip install virtualenv

## Building steps

### Environment(s)

Handling a number of multiple virtual environments can be a major pain - but there is hope, called [virtualenvwrapper](http://pypi.python.org/pypi/virtualenvwrapper).
Setup is really easy, please consult the docs. After you installed the wrapper, play around a little to catch up with the commands.

Here is my modifications for virtualenvwrapper's global hook, postmkvirtualenv: [http://gist.github.com/312660](http://gist.github.com/312660)
Nothing fancy, you can select a minimal or an advanced django development setup using one of my requirement files.

### Debugging

I found [django-devserver](http://github.com/dcramer/django-devserver) pretty nice with the optional packages like Werkzeug, guppy and sqlparse.

### Deployment

[Fabric](http://docs.fabfile.org/0.9.0/) is a simple tool to manage your deployments. It has customizable pre and post hooks sou you can run your apache reload scripts seamlessly.

## Useful links

## Thanks