# Node-RED Starter Kit

## Overview

[Node-RED Starter Kit](https://github.com/eqot/node-red-starter-kit)
is a boilerplate for IoT development with [Node-RED](http://nodered.org/).


## Background

A lot of websites about Node-RED including [the official site](http://nodered.org/)
let us install Node-RED globally by running ```npm install -g node-red```.
Also, all flow files and setting file are stored under home directory ```~/.node-red/```
by default.

This is good for quickstart but not good for portability of flows and its dependent modules.

So, this starter kit is developed for installing Node-RED and dependent modules locally,
and managing all files locally.
This enables to make flows potable and also run multiple flows on a single machine.


## Prerequisites

* [Node.js](https://nodejs.org/) (0.10.x or later)


## Features

* External nodes integration
  * Run ```npm install XXX --save``` for the external node to be available in the Node-RED editor
* Auto restart
  * Run ```npm run dev``` to watch changes under ```data``` directory and automatically restart the Node-RED server when changed
* Lint
  * Run ```npm run lint``` with [ESLint](http://eslint.org/)


## Quickstart

```
$ git clone https://github.com/eqot/node-red-starter-kit.git
$ cd node-red-starter-kit
$ npm install
$ npm start
```

Then local server is up and running at http://localhost:1880/.

If you want to follow all changes in this git repository, run followings instead of the above commands.

```
$ mkdir myFlow
$ cd myFlow
$ git init
$ git remote add upstream https://github.com/eqot/node-red-starter-kit.git
$ git fetch upstream master
$ git merge upstream/master
$ npm install
$ npm start
```

By running git fetch and merge, you can get the latest code.
