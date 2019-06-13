all: build push
.PHONY: build push

TAG = centos7

DOCKER_REGISTRY = harbor.top.mw/library

build:
	docker build -t $(DOCKER_REGISTRY)/ansible:$(TAG) .

push:
	docker login -u admin -p Harbor12345 harbor.top.mw
	docker push $(DOCKER_REGISTRY)/ansible:$(TAG)
	docker rmi -f $(DOCKER_REGISTRY)/ansible:$(TAG)
	docker logout harbor.top.mw