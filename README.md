openPMD Tools
=============

This repository contains scripts and small tools that can be used to work with
or enhance valid openPMD files.
See the [openPMD standard](https://github.com/openPMD/openPMD-standard).


More than Scripts
-----------------

If you are looking for libraries, projects and frameworks that support the
openPMD standard, please refer to our official list
[here](https://github.com/openPMD/openPMD-standard#projects-and-libraries).


Low-Level APIs & Libraries
--------------------------

Low-level tools for the underlying file formats that can be used with openPMD
flavoured files can of course still be used!

For **HDF5** these are (at least):

- GUI: [HDFView](https://www.hdfgroup.org/products/java/hdfview/),
       [HDF Compass](https://github.com/HDFGroup/hdf-compass)
- Python::Numpy binding: [`h5py`](http://www.h5py.org)
- Official [binary tools](https://www.hdfgroup.org/products/hdf5_tools/):
    [`h5ls`](https://www.hdfgroup.org/HDF5/Tutor/cmdtoolview.html#h5ls),
    [`h5dump`](https://www.hdfgroup.org/HDF5/Tutor/cmdtoolview.html#h5dump),
    `h5repack`, `gif2h5`, ...

an for **ADIOS**:

- Python::Numpy binding: `adios` and `adios_mpi`
- Official [binary tools](https://github.com/ornladios/ADIOS/tree/master/utils):
    `bpls`, `bpdump`, `bpmeta`, `bpdiff`, ...


Development
-----------

The development of these scripts is carried out *per-branch*.
Each branch corresponds to a certain version of the standard and might
be updated in case we find bugs or add new features.
