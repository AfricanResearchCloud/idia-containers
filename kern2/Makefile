IMAGE=kern-2.img

.PHONY: bootstrap

all: bootstrap

# Increased the storage allocation for KERN2. The default of 10GB was not enough. 
${IMAGE}:
	sudo singularity create -s 20000 ${IMAGE}

bootstrap: ${IMAGE}
	sudo singularity bootstrap ${IMAGE} os-default-ubu16.def 

upgrade:
	sudo singularity exec --writable ${IMAGE} apt-get update
	sudo singularity exec --writable ${IMAGE} apt-get upgrade
