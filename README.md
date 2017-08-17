#Setting up a new project
```
$ npm init - starting point to create a new package.json for a project
$ npm init -y - create a package.json with defaults
$ npm set/get - set defaults for fields 
$ npm install - install all project dependencies from package.json
$ npm start - run any script included in scripts : start in package.json
$ npm test - run any test scripts listed in package.json
```

#Getting help
```
$ npm help <command> - opens up docs for command in browser, loded from a local copy of command docs.
$ npm help-search <search-term> - lists out matching terms from docs
```

#Installing/Uninstalling/Updating Packages
```
$ npm install <package-name> - install a new package
$ npm install <package-name> -S - install a new package and save to package.json
$ npm install <package-name> -g - install a new package globally,this does not install packages in the project dir. 
$ npm install <package-name@version> - install package at a specific version
```
##version semantics:   
command flags::  
@1.7 - latest version at minor 1.7.x  
@1.x - latest minor  
package.json dependencies::  
@">=1.1.0 <1.4.0...add more boolean compound terms" - Anything that falls between 1.1.0 & 1.4.0  
"^1.8.3" - install latest version of major release whenever npm install is invoked, remove ^ or use --save-exact flag to prevent npm     from installing latest version.
"~1.8.3" - latest version of minor release when npm install is invoked.  
"\*" - always update to latest, minor/major/*  
```
$ npm install <dev-only-package> -D - install and add a package to dev dependencies, eg karma
$ npm uninstall <package-name> - This will uninstall package, package name will still persist in package.json, add -g flag for global package
$ npm uninstall <package-name> --save - Uninstall and remove from package.json 
$ npm update --dev/prod - update dev/prod dependencies, no flags, update all dependencies. 
```
Semantic versioning for packages: Major(new features added that are not backwards compatible, can break existing code).Minor(new features added, usually backwards compatible, does not braek existing code).Revision(Patch fix/Bug fix/Performance improvement)

#Listing Packages
```
$ npm list - Prints out project dependencies as a tree.
$ npm list --depth 0 - Prints out project dependencies installed by developer.
$ npm list --global true - Prints out project dependencies installed globally, can be combined with depth flag.
$ npm list --long true - Prints out project dependencies with some extra info.
$ npm list --dev true - Prints out project dev dependencies.
$ npm list --json true - Prints out project dependencies in json format.
```
