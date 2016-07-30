# Download Manager Packages
This is a package repository for hosting packages for the download manager

## Root
At the root is `manifest.json`. This file holds the list of packages and home registry entries for each package

## Package
A package is zipped in a specific way.

`checkmate-2.3.8.zip` 
| Application Name | Version | Archive Type |
| :--------------: | :-----: | :----------: |
|    checkmate     |  2.3.8  |     zip      |

Application name and version are separated by a `-` and end in `.zip` since Zip archives are the only one supported at the moment

## Package Contents
For now, only installers are supported. A more customizable way of installing without an installer will be added later, but not now. A package currently contains 2 files:  
* Installer
* manifest.json

The installer is just that, the application installer. Any installer will work. `manifest.json` contains the package's definitions, required packages, and installer options

## Prerequisites
[Microsoft .NET 4.5](https://www.microsoft.com/en-us/download/details.aspx?id=30653) is required to run the download manager
