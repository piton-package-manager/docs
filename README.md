Piton is a python package manager modelled after NPM. Piton makes it easier for Python developers to share and reuse code.

## Features

- Piton keeps track of your development dependecies
- Piton keeps track of production dependecies
- Piton allows you to define project specific scripts (for testing, deploying, etc.)

## Getting Started

To start, run:
```
piton init
```
The init command will add piton to your current project

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

## Updating Packages

To update a package, simply change the version of the package in your package.json file and then run:
```
piton install
```

## User Defined Scripts

You can add custom scripts to your package.json file and you can run them running `piton <script_name>`

```
"scripts": {
    "start": "python3 manage.py runserver",
    "deploy": "git push origin master"
  }
```

## Version Control 

Add the following to your package.json file for your version control details

```
"repository": {
  "type": "<TYPE>",
  "url": "<REPO_URL>"
}
```

## Issue Tracking

Piton supports Gitlab, Githuba and Jira issue trackers. First add your issue tracker to the package.json file:
```
"bugs": {
  "url": "https://github.com/nodejitsu/browsenpm.org/issues"
}
```

To browse all issues run:
```
piton issues
```

To browse issues assigned to you run:
```
piton issues --assignee me
```

To browse through issues assigned to someone else run:
```
piton issues --assigne <username>
```

To filter issues run:
```
piton issues --filter <search_term>
```


