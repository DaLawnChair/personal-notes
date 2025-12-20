

Package Manager: a library built for installlation and maininting of an deveopment environment.



Pip is the builtin package manager that comes with most python packages. 
Recursively defined name: Pip Installs Packages
Availability: Python3.4+


Pip installs packages natively hosted on Python Package Index (PyPI), as well as explicitly in Github and local repositories.


Usage:
```python
# Calling pip. All of these can be equivalent if used in a single environment
pythom -m pip
pip 
pip3 
# NOTE: these commands can have different aliases and can download to different enviornments or from different caches. Check with `which <command>` to verify that it is the correct verson 


--help == list out the available commands
--version == current version of pip used

```



# Installation
```python

# installation of a package
pip install <name> ... <name>
-r == pull from a .txt file
-U --upgrade == upgrade this package to the newest available version

-e <path or url> == local project path, or Version Control Source (VCS) version like Github
--no-deps == do not install package depdendencies

--dry-run == don't install anything, just print as if it does
-t --target <dir> == install from a directory, will not upgrade that directory unless -U is specified
--platform <platform> == only use wheel files compatible with that platform


--upgrade-strategy <upgrade_strategy> == determines how the packages are upgraded:
1. only-if-needed (default) == only upgrade if not already satisfactory
2. eager == upgraded depdendencies regardless if the installed version is already satisfactory

--force-reinstall == reinstall all packages, even if already up to date
-I --ignore-installed == ignore the following packages. Can break your environment

--no-build-isolation == Disable isolation when building a modern source distribution. This ignores the temporary environment used to build the package, and instead builds it directly into your enviornment. Must have the depdendencies already installed.
 

```

Internally, `pip install` goes through the following stages:
	1. Identification of base requirements (like the passed package names)
	2. Resolve Depdendencies, determines what is installed
	3. Build Wheels. Finds all dependencies that can be installed as .whl files
	4. Install the packages (uninstalling and upgrading anything that is needed)

Arguments are checked for types:
1. project urls or achive urls
2. local directory (specified by `pyproject.toml` or `setup.py`)
3. local file ( a sdist file (ie .tar.gz) or .whl )
4. version specified (ie `flash_attn==2.8.3`)
	1. Packages are worked out from their file names (for sdist and wheel files) or their setup.py egg_info metadata

Once pip has found the packages and depdendencies, it will try to resolve the dependencies based on the rules:
1. lastest released version of a package will be installed that satisfies the requirements of all packages
2. It will only install stable versions for the package (from pip version 1.4 onward), unless 
	1. the requirement specifier denotes a developer or prerelease version (ie `>=0.0.dev0`) 
	2. pip install is used with  the `--pre` flag

Pip installs packages by the dependencies first, and then the depdendents (in topological order).
Ordering of the packages in `pip install` is not guarenteed. This is because this order is likely to leave an environment working if a failed installation occurs, and the environment can be used during installation.


During circular depdendencies, first encountered member of the cycle is installed last.



Reporting:
`--report` generates a `.json` file file for the installation. Use this with `--dry-run` and `--ignore-installed` to get a resolve set of requirements before installing.


Reference:
https://pip.pypa.io/en/stable/cli/pip_install/


# uninstall a package
pip uninstall <name> ... <name> 