all: build push
.PHONY: build push

TAG = 1.7.6

DOCKER_REGISTRY = harbor.top.mw/library

build:
	docker build --no-cache -t $(DOCKER_REGISTRY)/kubectl:$(TAG) .

push:
	docker login -u admin -p Harbor12345 harbor.top.mw
	docker push $(DOCKER_REGISTRY)/kubectl:$(TAG)
	docker logout harbor.top.mw