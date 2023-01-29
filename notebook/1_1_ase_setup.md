# Setup

## Install ASE+GPAW

GPAW work interactively with ASE

GPAW only works on Linux environment.

Can use with WSL, python=3.10

Use `clang` to replace `gcc`; and install all packages from `conda-forge`, then they can linked to each other

```sh
conda install -c conda-forge clang lld llvm-tools openmpi llvm-openmp blas libxc scalapack fftw libvdwxc elpa ase gpaw
```

**Test**
Run in env `py310ase`

```sh
gpaw test
```

```{note}
- [fix GPAW_SETUP_PATH](https://jensj.gitlab.io/gpaw-2021-talk/slides/slide-09.html)
  ```sh
  gpaw install-data --register ~/PAWDATA
  ```

- Avoid install from source using `pip`, since it can not link with `scalapack fftw libvdwxc elpa` from conda-forge

  ```sh
  pip install --upgrade git+https://gitlab.com/ase/ase.git@master
  pip install --upgrade  git+https://gitlab.com/gpaw/gpaw.git
  ```

- Use `clang lld llvm-tools` to instead `gcc=12 gxx=12 libstdcxx-ng=12`

  ```sh
  conda install -c conda-forge gcc=12 gxx=12 libstdcxx-ng=12
  conda install -c conda-forge  openmpi openmp blas libxc scalapack fftw libvdwxc elpa
  ```

```

```{seealso}
1. [Installation ASE](https://wiki.fysik.dtu.dk/ase/install.html)
2. [Installation GPAW](https://wiki.fysik.dtu.dk/gpaw/install.html)
```
