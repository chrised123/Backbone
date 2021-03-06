# Backbone

[![Twitter Follow](https://img.shields.io/twitter/follow/forCrowd.svg?style=social)](https://twitter.com/forCrowd)
[![Join the chat at https://gitter.im/forCrowd/Backbone](https://badges.gitter.im/forCrowd/Backbone.svg)](https://gitter.im/forCrowd/Backbone?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

An API service for rapid app prototyping

## Current Stack

### Server

* .NET Framework 4.6
* ASP.NET Web API 2 & OData v3
* Entity Framework 6
* SQL Server 2014

### Client

* Angular
* Angular CLI
* TypeScript
* BreezeJS
* Karma & Jasmine

## Setup

Follow this document to setup the application on your computer:  
[Getting Started](https://github.com/forcrowd/Backbone/wiki/Getting-Started)

## Deployment

### Server (WebAPI)

You can deploy WebApi appliation through Visual Studio publish.  

Only remark is, configuration files are excluded from deploy (Build Action: 'None').  
When deploying the project, update following configuration files with your own settings and manually copy them:
* WebApi\googleanalytics.js
* WebApi\Web.config
* WebApi\Configs\\*.config

If you would like to make the application offline during the deployment, you can use **app_offline.htm_**.

### Client (AngularClient)

AngularClient is a Angular CLI project and all of its commands are available.

Thera are three environments defined in `.angular-cli.json` file: `dev`, `test` & `prod`.  
For `test` & `prod`, please create your own files by copying `dev` configuration file:

    AngularClient\src\app-settings\environments\environment-settings.ts

To prepare a production bundle, run the following on your command console:

    ng build -prod

For more options, please visit [Angular CLI](https://github.com/angular/angular-cli)

## Contribute

### First Mission: Contributors Page
This is an experimental attempt to help you to get familiar with our project and make your first pull request.

Follow the document for detailed instructions:
[First Mission](https://github.com/forCrowd/Backbone/wiki/First-Mission)

## Changelog

See [Changelog.md](/CHANGELOG.md) for a detailed list.

## License

Backbone is licensed under [MIT license](/LICENSE).
