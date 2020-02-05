# PROJ

[![Travis Status](https://travis-ci.com/OSGeo/PROJ.svg?branch=master)](https://travis-ci.com/OSGeo/PROJ)
[![AppVeyor Status](https://ci.appveyor.com/api/projects/status/github/OSGeo/PROJ?branch=master&svg=true)](https://ci.appveyor.com/project/OSGeo/PROJ?branch=master)
[![Coveralls Status](https://coveralls.io/repos/github/OSGeo/PROJ/badge.svg?branch=master)](https://coveralls.io/github/OSGeo/PROJ?branch=master)
[![Gitter](https://badges.gitter.im/OSGeo/proj.4.svg)](https://gitter.im/OSGeo/proj.4)
[![Mailing List](https://img.shields.io/badge/PROJ-mailing%20list-4eb899.svg)](http://lists.osgeo.org/mailman/listinfo/proj)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v1.4%20adopted-ff69b4.svg)](CODE_OF_CONDUCT.md)

PROJ is a generic coordinate transformation software, that transforms
coordinates from one coordinate reference system (CRS) to another.
This includes cartographic projections as well as geodetic transformations.

For more information on the PROJ project please see the web page at:

https://proj.org/

The PROJ mailing list can be found at:

https://lists.osgeo.org/mailman/listinfo/proj/

See the NEWS file for changes between versions.

The following command line utilities are included in the PROJ package:

- `proj`: for cartographic projection of geodetic coordinates.
- `cs2cs`: for transformation from one CRS to another CRS.
- `geod`: for geodesic (great circle) computations.
- `cct`: for generic Coordinate Conversions and Transformations.
- `gie`: the Geospatial Integrity Investigation Environment.
- `projinfo`: for geodetic object and coordinate operation queries.
- `projsync`: for synchronizing PROJ datum and transformation support data.

> More information on the utilities can be found on the [PROJ website](https://proj.org/apps).

## Installation

Consult the [Installation](https://proj.org/install.html) page of the official
documentation.
For builds on the master branch, [install.rst](https://github.com/OSGeo/PROJ/blob/master/docs/source/install.rst)
might be more up-to-date.

## Distribution files and format

Sources are distributed in one or more files.  The principle elements
of the system are stored in a compressed tar file named `proj-x.y.z.tar.gz` where
"x" will indicate the major release number, "y" indicates the minor release
number, and "z" indicates the patch number of the release.

In addition to the PROJ software package, distributions of datum
conversion grid files and PROJ parameter files are also available.
The grid package is distributed under the name `proj-datumgrid-x.y.zip`,
where "x" is the major release version and "y" is the minor release
version numbers. Similarly regional packages are distributed. The
regional packages contain resources that are not essential to the
functionality of PROJ but still of value to users in the region
specific to the package. All grids that were in proj-datumgrids-1.6
remain in proj-datumgrids-1.7; the regional datumgrid files contain
grids for datums not previously supported (prior to PROJ 5.0.0).

The resource packages can be downloaded from the [PROJ website](https://proj.org/download.html).

More info on the contents of the various resource packages can be
found at the
[proj-datumgrid GitHub repository](https://github.com/OSGeo/proj-datumgrid).

The resource file packages should be extracted to `PROJ_LIB`
where PROJ will find them after installation. The default location of
`PROJ_LIB` on UNIX-based systems is `/usr/local/share/proj` but it may
be changed to a different directory. On Windows you have to define
`PROJ_LIB` yourself.

## Citing PROJ in publications

See [CITATION](CITATION)
