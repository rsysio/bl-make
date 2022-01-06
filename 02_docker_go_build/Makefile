GO_VERSION := 1.17.5

hello:
	docker run -v ${PWD}:/app \
		-w /app \
		golang:$(GO_VERSION) \
		go build hello.go
