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

#Installing Packages
```
$ npm install <package-name> - install a new package
$ npm install <package-name> -g - install a new package globally,this does not install packages in the project dir. 
$ npm install <dev-only-package> -D - install and add a package to dev dependencies, eg karma
```

#Listing Packages
```
$ npm list - Prints out project dependencies as a tree.
$ npm list --depth 0 - Prints out project dependencies installed by developer.
$ npm list --global true - Prints out project dependencies installed globally, can be combined with depth flag.
$ npm list --long true - Prints out project dependencies with some extra info.
$ npm list --dev true - Prints out project dev dependencies.
$ npm list --json true - Prints out project dependencies in json format.
```
