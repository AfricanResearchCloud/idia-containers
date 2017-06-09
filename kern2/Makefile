IMAGE=kern-2.img
DEF=kern-2.def

.PHONY: bootstrap

all: bootstrap

# Increased the storage allocation for KERN2 to 20GB. The default of 10GB was not enough. 
${IMAGE}:
	sudo singularity create -s 20000 ${IMAGE}

bootstrap: ${IMAGE}
	sudo singularity bootstrap ${IMAGE} ${DEF}

upgrade:
	sudo singularity exec --writable ${IMAGE} apt-get update
	sudo singularity exec --writable ${IMAGE} apt-get upgrade
