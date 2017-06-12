# IDIA Software Containers - Singularity 

Inter University Data Intensive Astronomy repository which contains the singularity definition files for building the containers

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

[link](http://singularity.lbl.gov/ "Singularity") 
```
Give examples
```

### Installing

A step by step series of examples that tell you have to get a development env running

Install Singularity from

```
VERSION=2.3
wget https://github.com/singularityware/singularity/releases/download/$VERSION/singularity-$VERSION.tar.gz
tar xvf singularity-$VERSION.tar.gz
cd singularity-$VERSION
./configure --prefix=/usr/local
make
sudo make install
```
