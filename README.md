*SportChef Web Frontend*
========================

[![Build Status](https://travis-ci.org/sportchef/sportchef-frontend.svg?branch=master)](https://travis-ci.org/sportchef/sportchef-frontend)  [![Stories in Ready](https://badge.waffle.io/sportchef/sportchef-frontend.svg?label=ready&title=Ready)](http://waffle.io/sportchef/sportchef-frontend) [![gitmoji](https://img.shields.io/badge/gitmoji-%20😜%20😍-FFDD67.svg)](https://gitmoji.carloscuesta.me)

**This repository contains the code for the microservice delivering the web frontend for the *SportChef* project. For more information please take a look at our [project website](https://www.sportchef.ch/).**

*Copyright (C) 2015, 2016 Marcus Fihlon*

This program is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.

## Running *SportChef*

### Using Docker

First, you have to create a network where all the running *SportChef* container instances can communicate with each other. You only need to do this once:

`docker network create sportchef`

The *sportchef/sportchef-frontend* docker image is available on DockerHub. To run *sportchef-frontend*, you have to specify the mode (e.g. `-d` for detached), network (e.g. `sportchef`) and a port mapping to map the ports of the web server inside the container (always `80`) to a port on your machine (e.g. `8080`). The complete docker call looks like this:

`docker run -d --net sportchef -p 8080:80 sportchef/sportchef-frontend`

### Building Docker locally

To build an own image of *sportchef-frontend*, you have to give it a name (tag it, e.g. `sportchef-frontend`) and to specify the directory containing the `Dockerfile` (e.g. `.` for the current working directory). The complete docker call looks like this:

`docker build -t sportchef-frontend .`

## Throughput

[![Throughput Graph](https://graphs.waffle.io/sportchef/sportchef-frontend/throughput.svg)](https://waffle.io/sportchef/sportchef-frontend/metrics/throughput)
