all: build push
.PHONY: build push

TAG = 1.13.6.2-centos

DOCKER_REGISTRY = harbor.top.mw/library

build:
	docker build --no-cache -t $(DOCKER_REGISTRY)/openresty:$(TAG) .

push:
	docker login -u admin -p Harbor12345 harbor.top.mw
	docker push $(DOCKER_REGISTRY)/openresty:$(TAG)
	docker logout harbor.top.mw