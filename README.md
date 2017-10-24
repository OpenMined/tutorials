# Tutorials

> OpenMined is an unincorporated, volunteer-only open source project to provide federated machine learning using blockchain technology.

This repository provides tutorial code to explore and learn various projects in the openmined ecosystem.

<!-- TOC depthFrom:2 -->

- [Prerequisites](#prerequisites)
- [Contents](#contents)
    - [Basics](#Basics)
    - [Intermediate](#Intermediate)
    - [Advanced](#Advanced)
- [For contributors](#For-Contributors)
- [Community](#Community)
- [License](#License)

<!-- /TOC -->

## Prerequisites

- Make sure Python 3.5+ is installed on your machine by checking `python3 --version`
- Set up a virtual environment for the Python libraries (optional, recommended)
- Install pysyft by following the instructions listed over [here](https://github.com/OpenMined/PySyft/blob/master/README.md)
- Install pysonar by following the instructions listed over [here](https://github.com/OpenMined/PySonar/blob/master/README.md)
- Install capsule by following the instructions listed over [here](https://github.com/OpenMined/Capsule/blob/master/README.md)

### Virtual Environment Setup
Although this step is optional, it is highly recommended. We will cover a few of the different ways in which they can be setup. Choose the one that is the most suitable for your environment.

- [Python3 VENV](#python3-venv)
- [Anaconda Create](#anaconda-create)
- [Virtualenv Wrapper](#virtualenv-wrapper)

The first thing to do is to navigate to the directory where you would like to keep the project and then create the virtual environment there:

```bash
mkdir OpenMined;
cd OpenMined
```

#### Python3 VENV
Since venv isn't standard until Python 3.6 we should make sure that we have the package installed if using a version of Python lower than that. I would recommend using your system's package manager to keep things tidy:

`sudo apt-get install python3-venv`

Once you've confirmed that you have *venv*, to create your virtual environment the command is as follows:

`python3 -m venv OpenMined`

Standard convention is to create a virtual environment with the name of *.venv*, but I like to see the name of the environment so that I am sure that I have the correct one active.

To **activate** the environment:

`source OpenMined/bin/activate`

You will know that you have done it correctly when the name *(OpenMined)* appears at the beginning of your prompt.

To **deactivate** the environment:

`deactivate`

#### Anaconda Create
The easiest way would be to clone your root environment. This way all of the packages that come with Anaconda will be available to you without having to install them one at a time:

`conda create -n OpenMined --clone root`

If you would like more control over the packages in your virtual environment, I would recommend `conda create --help` or the online [documentation](https://docs.anaconda.com/docs_oss/conda/using/envs#).

To activate/deactivate the environment:

```bash
# Linux
source activate OpenMined
source deactivate
```
```shell
# Windows
activate OpenMined
deactivate
```
#### Virtualenv Wrapper
Complete instructions on how to install [virtualenv](http://docs.python-guide.org/en/latest/dev/virtualenvs/) and [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/) is beyond the scope of these instructions, but will make things easier with managing your environments.

If you have *virtualenv* and *virtualenvwrapper* installed, then you might want to use either one of these steps:

```bash
mkvirtualenv -p python3 OpenMined
setvirtualenvproject
```
or:

```bash
mkproject -p python3 OpenMined
```
Either will set your current working directory as the project folder for the virtual environment, so that when you activate it, you will automatically start in that directory.

To activate/deactivate:

```bash
workon OpenMined
deactivate
```

## Contents

### [Basics](https://github.com/OpenMined/tutorials/tree/master/beginner)
- [Pysonar-Decentralized model training simulation](https://github.com/OpenMined/tutorials/blob/master/beginner/Pysonar-Decentralized%20model%20training%20simulation.ipynb)
- [Pysyft-Paillier Homographic Encrypted Linear Classification](https://goo.gl/86M4bg)
### [Intermediate]() [WIP]
### [Advanced]() [WIP]


## For Contributors

If you are interested in contributing to this, first check out our [Contributor Quickstart Guide](https://github.com/OpenMined/Docs/blob/master/contributing/quickstart.md) and then sign into our [Slack Team](https://openmined.slack.com/)  to let us know which projects sound interesting to you! (or propose your own!).

Here's how you can contribute:

we would like to explore every possible use of the Openmined ecosystem and share these with the community, To that end you can create various tutorials and Put it in one of the _beginner_, _intermediate_, _advanced_  sections based on their appropriate levels.

You can raise an issue or submit a pull request, whichever is more convenient for you.

## Community

1. [Slack](https://openmined.slack.com/)

## License

[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
