<img align="left" width="200" src="src/assets/transitsphere_logo.png"> 

# TransitSphere
### _Civic Guide of Seattle Transportation Ecosystem_

[![Build Status](https://travis-ci.org/ibromley/sdot-webcomp.svg?branch=master)](https://travis-ci.org/ibromley/sdot-webcomp)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)


> As the fastest growing city in the nation, Seattle’s transportation system is under tremendous stress. Whether we walk, bike, or drive, we all share the same road. However, information about our transportation system is often hard to find and confusing to interested citizens. TransitSphere, built in partnership with Seattle Department of Transportation, serves as a civic guide to the assets SDOT manages. The experience this tool provides allows citizens to learn more about their transit infrastructure in a way that is both approachable and informative.


Live demo: [https://ibromley.github.io/sdot-webcomp/](https://ibromley.github.io/sdot-webcomp/)

Data Source: [https://docs.google.com/spreadsheets/d/1-aBL2tsKYet1vlc4ESGTYoNmt7wzVoDdmzv3PKZWjkU/](https://docs.google.com/spreadsheets/d/1-aBL2tsKYet1vlc4ESGTYoNmt7wzVoDdmzv3PKZWjkU/)

SDOT Status and Condition Report: [2015 Status & Condition Report](http://www.seattle.gov/Documents/Departments/SDOT/About/SDOT2015SCReportFinal12-7-2015.pdf)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Make sure you have installed all of the following prerequisites on your development machine:

* Git - [Download & Install Git](https://git-scm.com/downloads). OSX and Linux machines typically have this already installed.
* Node.js - [Download & Install Node.js](https://nodejs.org/en/download/) and the npm package manager.
* Grunt - [Download & Install Grunt](https://gruntjs.com/) the javascript task runner. You can download and install it by simply using npm. 
```
npm install -g grunt-cli
```

### Installing

The recommended way to get TransitSphere is to use `git` to directly clone the repository to your localmachine:

```
$ git clone https://github.com/ibromley/sdot-webcomp sdot-webcomp
$ cd sdot-webcomp
```
```
# install dependencies
npm install

# build project directory
npm run build
```

## Deployment

Builds can be pushed to Github Pages by invoking the `gh-pages` grunt task:

```
$ grunt gh-pages
```

## Built With
* [Less](http://lesscss.org/) - CSS preprocesor
* [Lodash](https://lodash.com) - HTML templating
* [NPM](https://www.npmjs.com/) - Dependency Management
* [Grunt](https://gruntjs.com/) - Our task runner

## Authors

* **Iain Bromley** - *Development* - [ibromley](https://github.com/ibromley)
* **Linh Tran** - *UI/UX Design* - [ltran1118](https://github.com/ltran1118)
* **Patrick Smith** - *Project Managment* [psmith94](https://github.com/psmith94)
* **Ryker Schwartzenberger** - *Development* - [rykerls](https://github.com/rykerls)

See also the list of [contributors](https://github.com/ibromley/sdot-webcomp/contributors) who participated in this project.

## License

This project is licensed under the MIT License - see the [LICENSE.txt](./LICENSE.txt) file for details

## Acknowledgments

* Props to the [Asset & Performance Management](http://www.seattle.gov/transportation/about-sdot/asset-management) team at the Seattle Department of Transportation for allowing us to paricipate on this project
* Thanks to the Seattle Times for the awesome [project template](https://github.com/seattletimes/newsapp-template)
