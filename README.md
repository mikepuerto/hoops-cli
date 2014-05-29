#Hoops CLI

A command line utility for the [hoops](https://github.com/mikepuerto/hoops) framework. This utility allows you to easily create apps, models, services, and controllers, interfaces with the applications config and, assists with deployments.

## Table of Contents
* [Commands & Usage]()
* [Generators]()
* <span style="color: red;">Config Editor - Second/Third Phase</span>
* <span style="color: red;">Deployments - Second/Third Phase</span>

### Commands
* ```$ hoops - displays help menu```
* ```$ hoops generate(g)```
* ```$ hoops config(c) <path> - (i.e. hoops config server.port=3000) (add ENV switch to edit ENV specific config)```
* ```$ hoops deploy(d) - based on deploy config for current ENV```

### Generators
* ```$ hoops generate new <app-name> - creates a new app in a new directory <app-name>```
* ```$ hoops generate service <service-name> <property:type>  - creates a new data service with defined properties (including model) and uses the default controller```
* ```$ hoops generate model <model-name> <property:value> - creates a model alone with the defined properties```
* ```$ hoops generate controller <controller-name>```
* ```$ hoops generate route <patter:match/middleware-stack>```
* ```$ hoops generate config <config-name> <property:value>```

### Config Editor
* <span style="color: red;">```$ hoops config <env> <property:value>```</font>
* <span style="color: red;">```$ hoops config route <pattern:controller#method```</font>

### Deployments
* <span style="color: red;">```$ hoops deploy```</font>

*<sub>**NOTE:** ***for all generators and config editors, allow dot notation for nested object and implment something to hand arrays. i.e. params passed as <property:value>***</sub>