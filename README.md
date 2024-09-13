# conda-packaging-example

## What is conda?

"Conda is a cross-platform, language-agnostic binary package manager. It is the package manager used by Anaconda installations, but it may be used for other systems as well. Conda makes environments first-class citizens, making it easy to create independent environments even for C libraries. Conda is written entirely in Python, and is BSD licensed open source."

## 

build all projects

```
cd projects
rattler-build build  --recipe-dir .
```

build a single project

```
cd projects/a/
rattler-build build --recipe recipe.yaml
```

## Problems

* conda package file contains source files twice => packages are twice as big as it should be 500 MB => 1 GB. The installed conda package has the single size.
* owner and group are not supported
* mode 

## Problems using rpm

* dnf is for the os: 

## Resources

    * https://docs.conda.io/projects/conda/en/latest/
    * https://docs.conda.io/projects/conda-build/en/stable/install-conda-build.html
    * https://github.com/mamba-org/mamba
    * https://github.com/mamba-org/mamba
    * https://github.com/prefix-dev/rattler-build
    * https://prefix-dev.github.io/rattler-build/latest/
    * https://github.com/conda/rattler