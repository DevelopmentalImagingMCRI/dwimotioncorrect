---
layout: default
title: Using
---
<br>
<section class="content">
## Standard usage

```bash
DWIEddyCorrectMI -p -m transformfile dwi.nii.gz dwi_mc.nii.gz 0
```

* _-p_ enables parallel execution (optional)
* _-m_ specifies an output file for saving estimated transforms. Useful as a motion estimate.
* _dwi.nii.gz_ is the image file to be motion corrected
* _dwi\_mc.nii.gz_ is the output, corrected image file
* _0_ is the index of the image used as the reference in registration

Note that the order of parameters is important, with _-p_ and _-m_ appearing first, if used.

