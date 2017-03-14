# conda-chem-bioinfo-pkgs
Conda recipes for chem/bioinformatics packages

# PyMOL
PyMOL is an OpenGL based molecular visualization system

#### Install with conda:
```bash
conda install -c samoturk freeglut=3.0.0 
conda install -c mw pmw=2.0.1
conda install -c samoturk pymol=1.8.6.0 
```

##### Build
```bash
git clone https://github.com/samoturk/conda-chem-bioinfo-pkgs.git
conda build conda-chem-bioinfo-pkgs/pymol
```
You might have to add `samoturk` channel to build it so it resolves `freeglut` and `glew`. `conda config --add channels samoturk`
