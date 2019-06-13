all: build push
.PHONY: build push

TAG = 7.1.1

DOCKER_REGISTRY = harbor.top.mw/library

build:
	docker build -t $(DOCKER_REGISTRY)/filebeat:$(TAG) .

push:
	docker login -u admin -p Harbor12345 harbor.top.mw
	docker push $(DOCKER_REGISTRY)/filebeat:$(TAG)
	docker rmi -f $(DOCKER_REGISTRY)/filebeat:$(TAG)
	docker logout harbor.top.mw