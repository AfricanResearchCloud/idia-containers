## A Jupyter kernel for CASA
## https://github.com/aardk/jupyter-casa

IMAGE=idia-jupyter-casa.img
DEF=idia-jupyter-casa.def

.PHONY: bootstrap

all: bootstrap

${IMAGE}:
	sudo singularity create -s 6000  ${IMAGE}

bootstrap: ${IMAGE}
	sudo singularity bootstrap ${IMAGE} ${DEF}

upgrade:
	sudo singularity exec --writable ${IMAGE} apt-get update
	sudo singularity exec --writable ${IMAGE} apt-get upgrade
	sudo singularity exec --writable ${IMAGE} conda update --all

