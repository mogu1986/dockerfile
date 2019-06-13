all: build push
.PHONY: build push

TAG = 8-jdk-alpine

DOCKER_REGISTRY = harbor.top.mw/library

build:
	docker build -t $(DOCKER_REGISTRY)/java:$(TAG) .

push:
	docker login -u admin -p Harbor12345 harbor.top.mw
	docker push $(DOCKER_REGISTRY)/java:$(TAG)
	docker logout harbor.top.mw