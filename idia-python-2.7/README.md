# Anaconda Python 2.7 deployment within Singularity

Inter-University Data Intensive Astronomy repository which contain the singularity definition files for building singularity containers.

### Prerequisites

[Singularity](http://singularity.lbl.gov/ "Singularity")


### Installing Singularity

```
VERSION=2.3
wget https://github.com/singularityware/singularity/releases/download/$VERSION/singularity-$VERSION.tar.gz
tar xvf singularity-$VERSION.tar.gz
cd singularity-$VERSION
./configure --prefix=/usr/local
make
sudo make install
```

### Build Container  

```
git clone https://gitlab.com/africanresearchcloud/idia-containers.git
```

Change into any of the preferred container directories and execute ...
```
make 
```

This will now create a blank Singularity image and start the deployment inside the container based on the definition file. 

### Running the container 

```
singularity run <container_name> 
```
or 
```
./container_name
```
or 
``` 
singularity exec <container_name> <path_to_binary_inside_container>
```
 

