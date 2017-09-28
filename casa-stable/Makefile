IMAGE=casa-stable.img

.PHONY: bootstrap

all: bootstrap

${IMAGE}:
	sudo singularity create -s 10000 ${IMAGE}

bootstrap: ${IMAGE}
	sudo singularity bootstrap ${IMAGE} casa-stable.def

upgrade:
	sudo singularity exec --writable ${IMAGE} yum update 

clean:
	rm -f ${IMAGE}