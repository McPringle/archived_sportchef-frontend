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

The *sportchef/sportchef-frontend* docker image is available on DockerHub. To run *sportchef-frontend*, you have to specify a port mapping to map the ports of the application server inside the container (8080) to a port on your machine (e.g. 80) and you have to specify a folder on your machine to store the permanent data. The complete docker call looks like this:

`docker run -d -p [local port]:80 sportchef/sportchef-frontend`

### Building Docker locally

`docker build -t sportchef/sportchef-frontend .`

## Throughput

[![Throughput Graph](https://graphs.waffle.io/sportchef/sportchef-frontend/throughput.svg)](https://waffle.io/sportchef/sportchef-frontend/metrics/throughput)
