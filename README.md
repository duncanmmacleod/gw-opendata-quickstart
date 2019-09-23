# GW open data quickstart tutorial

This repository is a very short quickstart tutorial introducing the software tools needed to discover, download, and display open data from the Gravitational-Wave Open Science Center.

Notebooks 1 (`1-open-data`) and 3 (`3-gwpy-basics`) are adapted from those written by me for the second Gravitational-Wave Open Data Workshop (GWODW#2, Paris 2019) and reproduced here under the terms of the GPL-3.0-or-later license.

## Setting up a software environment to study GW open data

This document describes how to set up a software environment _from scratch_ in order to study gravitational-wave open data.

### 1. Install miniconda

GW software are conveniently distributed and installable with [Conda](https://docs.conda.io/). To get the `conda` package installer, install [Miniconda](https://docs.conda.io/en/latest/miniconda.html) following the instructions provided on that page.

### 2. Create a new environment in which to install GW software

It is good to use separate conda environments for each distinct software collection, so that things don't get muddled up. You can create a new environment and install software into it in one go:

```bash
conda create --name gwpy python=3.7 gwosc=0.4.3 gwpy=0.15.0 jupyter scipy=1.3.1
conda activate gwpy
```

### 3. Open jupyter notebooks using the new environment

```bash
jupyter notebook
```
