# openPMD-viewer

[![Build Status master](https://img.shields.io/travis/openPMD/openPMD-viewer/master.svg?label=master)](https://travis-ci.org/openPMD/openPMD-viewer/branches)
[![Build Status dev](https://img.shields.io/travis/openPMD/openPMD-viewer/dev.svg?label=dev)](https://travis-ci.org/openPMD/openPMD-viewer/branches)
[![pypi version](https://img.shields.io/pypi/v/openPMD-viewer.svg)](https://pypi.python.org/pypi/openPMD-viewer)
[![Number of PyPI Downloads](https://img.shields.io/pypi/dm/openPMD-viewer.svg)](https://pypi.python.org/pypi/openPMD-viewer)
[![License](https://img.shields.io/pypi/l/openPMD-viewer.svg)](LICENSE.txt)

## Overview

This package contains a set of tools to load and visualize the
contents of a set of [openPMD](http://www.openpmd.org/#/start) files
(typically, a timeseries).

The routines of `openPMD-viewer` can be used in two ways :

- Use the **Python API**, in order to write a script that loads the
  data and produces a set of pre-defined plots.

- Use the **interactive GUI inside the Jupyter Notebook**, in order to interactively
visualize the data.

## Usage

### Tutorials

The notebooks in the folder `tutorials/` demonstrate how to use both
the API and the interactive GUI. You can view these notebooks online
[here](https://github.com/openPMD/openPMD-viewer/tree/master/tutorials).

You can also download and run these notebooks on your local computer
(when viewing the notebooks with the above link, click on `Raw` to be able to
save them to your local computer). In order to run the notebook on
your local computer, please install `openPMD-viewer` first (see
below), as well as `wget` (`pip install wget`).

### Notebook quick-starter

If you wish to use the **interactive GUI**, the installation of
`openPMD-viewer` provides a convenient executable which automatically
**creates a new pre-filled notebook** and **opens it in a
browser**. To use this executable, simply type in a regular terminal:

`openPMD_notebook`

(This executable is installed by default, when installing `openPMD-viewer`.)

## Installation

### Installation on a local computer

Before installing `openPMD-viewer`, please make sure that `h5py` is
installed on your local computer. (If you are using the [Anaconda
distribution](https://www.continuum.io/downloads), this can be done by
typing `conda install h5py`. Otherwise, use `pip install h5py`, though
this may require you to install `hdf5` separately.)

Once `h5py` is installed, simply type
```
pip install openPMD-viewer
```

In addition, if you wish to use the interactive GUI, please type
```
pip install jupyter
```

### Installation on a remote scientific cluster

If you wish to install the `openPMD-viewer` on a remote scientific
cluster, please make sure that the packages `numpy`, `scipy` and `h5py`
are available in your environment. This is typically done by a set of
`module load` commands (e.g. `module load h5py`) -- please refer to
the documentation of your scientific cluster.

Then type
```
pip install openPMD-viewer --user
```

Note: The package `jupyter` is only required for the **interactive
GUI** and thus it does not need to be installed if you are only using
the **Python API**.  For [NERSC](http://www.nersc.gov/) users, access to Jupyter
notebooks is provided when logging to
[https://ipython.nersc.gov](https://ipython.nersc.gov).

## Contributing to the openPMD-viewer

We welcome contributions to the code! Please read [this page](https://github.com/openPMD/openPMD-viewer/blob/master/CONTRIBUTING.md) for
guidelines on how to contribute.
