## Please note that this repo is outdated and no longer maintained.  Newer versions of several of these container definition files may be found at https://github.com/idia-astro?q=idia-container or inside containers themselves at `/.singularity.d/Singularity`

# IDIA Software Containers

Inter-University Data Intensive Astronomy repository which contains the singularity definition files for building the containers

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

[Singularity](http://singularity.lbl.gov/ "Singularity")


### Installing Singularity

Install Singularity 

```
VERSION=2.3.1
wget https://github.com/singularityware/singularity/releases/download/$VERSION/singularity-$VERSION.tar.gz
tar xvf singularity-$VERSION.tar.gz
cd singularity-$VERSION
./configure --prefix=/usr/local
make
sudo make install
```
