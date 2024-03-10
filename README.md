# votings-hex-core
Votings application core based on hexagonal architecture.


## How to generate a package using a build system (setuptools)

Since this repo only uses the `pyproject.toml`, remember to use at least the version 61.0.0 of setuptools, or other package managers or build systems like hatchling, poetry, etc., that only needs `pyproject.toml`. (Modern python packers only needs pyproject.toml, there is no need of setup.py or setup.cfg) 

Remember to modify `pyproject.toml`, remplacing data for your package data. The file is prepared to be used by "setuptools" library. If you want to use other build system, remember to edit the `[build-system]` part.

For building the package (setuptools):
```bash
python -m pip install --upgrade pip setuptools wheel
python -m build

# And to install the package
python -m pip install --user dist/votings-hex-core-0.0.1.tar.gz
```