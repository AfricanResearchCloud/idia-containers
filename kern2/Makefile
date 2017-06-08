IMAGE=kern-2.img

.PHONY: bootstrap

all: bootstrap

${IMAGE}:
	sudo singularity create -s 10000 ${IMAGE}

bootstrap: ${IMAGE}
	sudo singularity bootstrap ${IMAGE} Singularity

upgrade:
	sudo singularity exec --writable ${IMAGE} apt-get update
	sudo singularity exec --writable ${IMAGE} apt-get upgrade

list:
	curl -s http://ppa.launchpad.net/kernsuite/kern-2/ubuntu/dists/xenial/main/binary-amd64/Packages.gz | zgrep Package | awk {'print $$2}' | xargs echo
