# Angular-deploy-project
This file describe how deploy a Angular project on github.com

## Requirement

You have already a project who's link with a github repository 

`git remote --verbose`

expected: an origin remote

`origin  https://github.com/<USERNAME>/<PROJECT_NAME>.git (fetch)`
`origin  https://github.com/<USERNAME>/<PROJECT_NAME>.git (push)`

If you don't have a repository

`git remote add origin https://github.com/<USERNAME>/<PROJECT_NAME>.git`

Make sure your repository is public in settings

## Install ghpages :

`npm i -g angular-cli-ghpages`

## Build your project :

`ng build --prod --base-href https://<USERNAME>.github.io/<PROJECT_NAME>/`

## Deployement
If you have `"outputPath": "dist/<PROJECT_NAME>"` in your angular.json file use 

`ngh --dir dist/<PROJECT_NAME>`

If you have `"outputPath": "dist/"` in your angular.json file use 

`ngh`

## Visibility

Your project is now available at:

`https://<USERNAME>.github.io/<PROJECT_NAME>/`

## Tools documentation :

|Tools  | Documentation| 
|--|--|
| Angular  | [https://angular.io/](https://angular.io/) |
| Git  | [https://www.npmjs.com/package/angular-cli-ghpages](https://www.npmjs.com/package/angular-cli-ghpages) |

