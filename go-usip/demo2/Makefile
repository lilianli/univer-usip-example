VERSION ?= latest

.PHONY: build image

build:
	@mkdir -p bin
	@GOARCH=amd64 go build -o bin/server-amd64 .
	@GOARCH=arm64 go build -o bin/server-arm64 .

image: build
	@docker buildx --builder=images-builder build --platform linux/arm64,linux/amd64 -t \
		univer-acr-registry.cn-shenzhen.cr.aliyuncs.com/release/usip-server:${VERSION} \
		--push .