# Node-RED Starter Kit

## Overview

[Node-RED Starter Kit](http://code.sonyericsson.net/node-red/node-red-starter-kit)
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


## Quickstart

```
$ git clone https://github.com/eqot/node-red-starter-kit.git
$ cd node-red-starter-kit
$ npm install
$ npm start
```

Then local server is up and running at http://localhost:1880/.
