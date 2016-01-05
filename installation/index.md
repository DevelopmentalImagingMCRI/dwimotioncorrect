---
layout: default
title: Installation
---
<br>
<section class="content">
# Installing DWIMotionCorrect
DWIMotionCorrect is a python script and doesn't require building. However
several prerequisites are required and must be installed.

## Prerequisites

1. git (for installation and easy updates)
1. FSL 5.x
1. python 2.7 and the following packages
	* _numpy_
	* _scipy_
	* _nibabel_
	* _distutils_
1. Gnu parallel (optional)

## Downloading

```bash
git clone https://github.com/DevelopmentalImagingMCRI/dwimotioncorrect.git
```

Updates to DWIMotionCorrect can be fetched using

``` bash
git pull
```

## Python prerequisites
Python libraries required can be installed using pip or your system package manager:

``` bash
apt-get install python-nibabel python-numpy python-scipy
```

or

``` bash
pip install nibabel scipy
```

