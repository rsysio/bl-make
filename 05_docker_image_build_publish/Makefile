GO_VERSION ?= 1.17.5
BUILD_IMAGE := golang

DOCKER_REPO := rsysio
DOCKER_IMAGE := hello-go
DOCKER_TAG ?= $(shell git rev-parse --short HEAD)

.PHONY: build run publish

build:
	docker build -t $(DOCKER_REPO)/$(DOCKER_IMAGE):$(DOCKER_TAG) .

run:
	docker run $(DOCKER_REPO)/$(DOCKER_IMAGE):$(DOCKER_TAG)

publish:
	docker push $(DOCKER_REPO)/$(DOCKER_IMAGE):$(DOCKER_TAG)
