GO_VERSION ?= 1.17.5
DOCKER_IMAGE ?= golang

hello:
	docker run -v ${PWD}:/app \
		-w /app \
		$(DOCKER_IMAGE):$(GO_VERSION) \
		go build hello.go
