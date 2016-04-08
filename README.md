Piton is a python package manager modelled after NPM. Piton makes it easier for Python developers to share and reuse code.

## Features

- Piton keeps track of your development dependecies
- Piton keeps track of production dependecies
- Piton allows you to define project specific scripts (for testing, deploying, etc.)

## Install/Uninstall Packages

To install a package, simply run:
```
piton install <package_name>
```
To install a package as a development dependacy, simply run:
```
piton install <package_name> --save-dev
```
To install a package as a production dependacy, simply run:
```
piton install <package_name> --save
```
To uninstall a package, simply run:
```
piton uninstall <package_name>
```
