# sectionproperties
a python package for the analysis of arbitrary cross-sections using the finite element method written by Robbie van Leeuwen. *sectionproperties* can be used to determine section properties to be used in structural design and visualise cross-sectional stresses resulting from combinations of applied forces and bending moments.

## Installation:

For more detailed installation instructions, refer to the [documentation](https://sectionproperties.readthedocs.io/).

### UNIX (MacOS/Linux):

```
$ pip install sectionproperties
```

### Windows

Install *meshpy* by downloading the appropriate [installation wheel](https://www.lfd.uci.edu/~gohlke/pythonlibs/#meshpy).

Navigate to the location of the downloaded wheel and install using pip:

```
$ cd Downloads
$ pip install MeshPy‑2018.2.1‑cp36‑cp36m‑win_amd64.whl
```

Once *meshpy* has been installed, *sectionproperties* can be installed:

```
$ pip install sectionproperties
```

## Documentation:

*sectionproperties* has a fully documented python API which you can find at [https://sectionproperties.readthedocs.io/](https://sectionproperties.readthedocs.io/). To read more about the theory behind the program, its implementation and some more examples, check out my blog at [https://robbievanleeuwen.github.io/](https://robbievanleeuwen.github.io/).

## Current Capabilities:

### Pre-Processor:
- [x] Python API
- [x] Custom section geometry input
- [x] Common section geometry generators
- [x] Multiple geometry merging
- [x] Geometry cleaning
- [ ] JSON input file
- [ ] .dxf import
- [x] Quadratic triangular mesh generation
- [x] Composite material properties

### Cross-Section Analysis:
- [x] Global axis geometric section properties:
  - [x] Area
  - [x] First moments of area
  - [x] Second moments of area
  - [x] Elastic centroid
- [x] Centroidal axis geometric section properties:
  - [x] Second moments of area
  - [x] Elastic section moduli
  - [ ] Yield moment
  - [x] Radii of gyration
  - [x] Plastic centroid
  - [x] Plastic section moduli
  - [x] Shape factors
- [x] Principal axis geometric section properties:
  - [x] Second moments of area
  - [x] Elastic section moduli
  - [ ] Yield moment
  - [x] Radii of gyration
  - [x] Plastic centroid
  - [x] Plastic section moduli
  - [x] Shape factors
- [x] Warping section properties:
  - [x] Torsion constant
  - [x] Warping constant
- [x] Shear section properties:
  - [x] Shear centre (elastic method)
  - [x] Shear centre (Trefftz's method)
  - [x] Shear areas (global axis)
  - [x] Shear areas (principal axis)
- [x] Cross-section stresses

### Solver:
- [x] Direct solver
- [x] CGS iterative solver
- [x] Sparse matrices

### Post-Processor:
- [x] Plot geometry
- [x] Plot mesh
- [x] Plot centroids
- [x] Plot cross-section stresses
- [ ] Generate cross-section report
- [ ] Export to Paraview

### Additional Modules:
- [ ] Optimisation
- [ ] Reinforced Concrete
- [ ] Steel
