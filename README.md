# Enabling coastal data science at continental scale

This repository contains an abstract submission about enabling coastal data science at
continental scale to [EGU 2023](https://www.egu23.eu/). The repository contains both  
the abstract (LaTeX) and self-explanatory preliminary IPython notebooks that
form the basis for the results that would be presented during the EGU 2023 Pangeo session. 

The study showcases the advantages of cloud-native workflows for coastal data-analyis
at continental scale by two examples. The first example estimates coastal assets at risk
of flooding by combining [building
footprints](https://github.com/microsoft/GlobalMLBuildingFootprints) with a coastal mask
that demarcates flood-prone areas along the European coast (Lincke et al., in press). In
the second example we benchmark data-proximate shoreline mapping against conventional
methods. 

## Installation

This study is built upon the [Pangeo core packages](https://pangeo.io/packages.html)
altogether with [Dask GeoPandas](https://dask-geopandas.readthedocs.io) and
[SpatialPandas](https://github.com/holoviz/spatialpandas). Thus, most used software is
directly available in [Pangeo docker
images](https://github.com/pangeo-data/pangeo-docker-images) and [Planetary Computer
containers](https://github.com/microsoft/planetary-computer-containers). 

On a local machine the software dependencies can be installed in a project environment
using `conda` or `mamba`. The file [environment.yml](./environment.yml) provides a list
of packages that are used or useful for analysis akin. To install these, run the
following command from the project root: 
```bash
mamba env create
```
This will create a new environment, named "coastal", that can be activated using: 
`mamba activate coastal`. 