# conda-chem-bioinfo-pkgs
Conda recipes for chem/bioinformatics packages

# PyMOL
PyMOL is an OpenGL based molecular visualization system

#### Install with conda:
[![Anaconda-Server Badge](https://anaconda.org/samoturk/pymol/badges/version.svg)](https://anaconda.org/samoturk/pymol) [![Anaconda-Server Badge](https://anaconda.org/samoturk/pymol/badges/downloads.svg)](https://anaconda.org/samoturk/pymol)

```bash
conda config --add channels conda-forge
conda install -c conda-forge glew=2.0.0
conda install -c samoturk freeglut=3.0.0 
conda install -c samoturk pmw=2.0.0
conda install -c samoturk pymol=1.8.6.0 
```

##### Build
```bash
git clone https://github.com/samoturk/conda-chem-bioinfo-pkgs.git
conda build conda-chem-bioinfo-pkgs/pymol
```
You might have to add `samoturk` and `conda-forge` channel to build it so it resolves `freeglut` and `glew`. `conda config --add channels samoturk`
