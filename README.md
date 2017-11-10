# Aurelia_bootstrap4_babel
Aurelia CLI .NET Core Webpack 3 - Bootstrap 4 - Babel (No TypeScript)

# Bootstrap 4 project (Aurelia, .NET Core 2.0, Webpack 3, Babel (NO TypeScript), Boostrap 4 and Sass)

This repository contains template for running Aurelia and ASP.NET Core 2.0 Sample Template, with Webpack 3, JavasScript, Bootstrap 4 and Sass.

### Setting Up Your Machine

First, there are a set of prerequisites you will need whether or not you are using Visual Studio. Make sure to install these prerequisites before proceeding.

* Install the .NET SDK 2.0 from https://www.microsoft.com/net/download/core
* [NodeJS](http://nodejs.org/) >=8.9.0 This provides the platform on which the build tooling runs. This may be downloaded and installed from the NodeJS website.
* NPM >=5.1.0 This is installed with NodeJS, but if you install a older version of NodeJS, you may have to update this. How to upgrade npm https://www.npmjs.com/package/npm-windows-upgrade
* Install Aurelia-CLI >= 0.32. How to install: `npm install aurelia-cli -g`


## How This Project Was Created

This prodject was created using the Aurelia CLI, width .NET Core 2.0
* `au new ` Aurelia CLI


## Running This Project Using Command Line Tools

In order to run this demo project, you need to setup your machine, restore the project dependencies, configure the environment and run the application.


###  Restoring The Project Dependencies

Since this project combines both .NET Core and Aurelia, you will need to install the dependencies for both the backend and the frontend. Here are the commands you need to run on the console:

* `npm install aurelia-cli -g` - Install aurelia-cli.
* `dotnet restore` - This restores the .NET packages for the ASP.NET part of the application.
* `npm install` - This restores the JavaScript packages that comprise Aurelia along with the related frontend build and development tooling, such as Webpack and TypeScript.
* `dotnet run` - Start url: http://localhost:5000 
* Or run Aureli-cli: `au build` then `au run`

#### Bug fix node-sass builde error!
If Node-sass was build for old node.js version, run:
* `npm rebuild node-sass --force -d` - This rebuild it for node 6 or 8.

#### Bug fix update old aurelia-cli to latest version!
* `npm uninstall -g aurelia-cli au`
* `npm cache clean`
* `npm install -g aurelia-cli`


If webpack build error:
* `FlagDependencyUsagePlugin.js const oldUsed = module.used`, then update Node (http://nodejs.org/) and NPM (https://www.npmjs.com/package/npm-windows-upgrade)


### Configuring Your Environment

* If you are using PowerShell on Windows, execute `$Env:ASPNETCORE_ENVIRONMENT = "Development"`
* If you are using cmd.exe on Windows, execute `setx ASPNETCORE_ENVIRONMENT "Development"`, and then restart your command prompt to make the change take effect.
* If you’re using Mac/Linux, execute `export ASPNETCORE_ENVIRONMENT=Development`


### Starting Up The Application

To run the application, simply execute `dotnet run` on the command line.


## Running This Project Using Visual Studio 2017

If you are on Windows, you have the option to use Visual Studio 2017 for your ASP.NET development. Simply use VS to open the .csproj file provided in this repository. 
When your dependencies have finished restoring, press Ctrl+F5 to launch the application in a browser.


### Third party documentation

* Bootstrap 4.0.0-beta.2 (http://getbootstrap.com/)
