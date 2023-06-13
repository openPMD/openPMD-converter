openPMD Converters
==================

This repository contains scripts and small tools that can be used to work with
or enhance valid openPMD files.
See the [openPMD standard](https://github.com/openPMD/openPMD-standard).

Software projects that support openPMD natively are catalogued in [openPMD projects](https://github.com/openPMD/openPMD-projects).

Conversion from/to openPMD
--------------------------

The following external repositories contain converters to/from openPMD files.

- openPMD <=> openPMD: `openpmd-pipe` is part of [openPMD-api](https://openpmd-api.readthedocs.io)
  - domain: convert between openPMD backends such as HDF5, ADIOS BP and JSON, multiplex stream or change iteration encodings
  - [repository](https://github.com/openPMD/openPMD-api) (LGPLv3+)
  - maintainers: F Poeschel @franzpoeschel, A Huebl @ax3l
  - status: implemented (base standard 1.X)

- [openPMD => VTK](https://github.com/hightower8083/opmd2VTK) (Weizmann Institute of Science, Israel)
  - domain: convert openPMD HDF5 to VTK containers
  - [repository](https://github.com/hightower8083/opmd2VTK) (GPLv3+)
  - maintainer: I Andriyash @hightower8083
  - status: implemented (base standard 1.X)

- [openPMD <=> GPT](https://github.com/KseniaBastrakova/openPMD-converter-GDF) (HZDR, Germany)
  - domain: convert between [GPT](http://www.pulsar.nl/gpt/)'s GDF and openPMD HDF5 (back & forth)
  - [repository](https://github.com/KseniaBastrakova/openPMD-converter-GDF) (ISC)
  - maintainers: K Bastrakova @KseniaBastrakova, A Huebl @ax3l
  - status: implemented (base standard 1.X)


More than Scripts
-----------------

This repository contains scripts and links to external projects that "heavily"
copy-convert between openPMD and other formats.

Please do not hesitate to contribute links to your own converters and scripts as a pull request.

If you are looking for libraries, projects and frameworks that support the
openPMD standard *out-of-the-box*, please refer to
[our official list](https://github.com/openPMD/openPMD-projects).


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

For **ADIOS1**:

- GUI: [HDF Compass](https://github.com/HDFGroup/hdf-compass)
- Python::Numpy binding: `adios` and `adios_mpi`
- Official [binary tools](https://github.com/ornladios/ADIOS/tree/master/utils):
    `bpls`, `bpdump`, `bpmeta`, `bpdiff`, ...

For **ADIOS2**:

- Python::Numpy binding: `adios2`
- Official [binary tools](https://adios2.readthedocs.io/en/latest/ecosystem/utilities.html):
    `bpls`, `bpdump`, `bpdiff`, ...
