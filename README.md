# Enhanced DWI motion correction

The repository contains the implementation of an enhanced version
of the FSL eddy correct tool that is designed to reduce registration
bias observed at b=3000. The method was described in:

_Improved Accuracy of Motion and Affine Eddy Current Distortion Correction in High B-Value Diffusion Weighted Imaging Using Brain Mask Based Weighting Functions_, Christopher Leslie Adamson, Richard Beare, Deanne Thompson, and Marc Seal, ISMRM 21st Annual Meeting and Exhibition, April 2013.

## Prerequisites

_DWIEddyCorrectMI_ is a python script with the following dependencies:

* python 2.7 and the following packages:
	* _numpy_
	* _scipy_
	* _nibabel_
	* _distutils_
* _FSL 5.x_
* _GNU Parallel_ (optional)

## synopsis

_DWIEddyCorrectMI_ [-p] [-m <output mat file>] <input file> <output file> <reference index>

Performs alignment of each volume in <input file> to the image in the input file specified by <reference index>; the first volume is 0

### Options
* -m <output mat file>: contains all of the transformation matrices concatenated
* -p use GNU parallel to perform the registrations in parallel, uses GNU parallel
