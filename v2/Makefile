IMG = e2eteam/k8s-ovn-ovs-ci
TAG = dev-terraform

all: build

build:
	@echo Build $(IMG):$(TAG)
	docker build -t $(IMG):$(TAG) .

push: build
	docker push $(IMG):$(TAG)
	docker image rm $(IMG):$(TAG)
	@echo Pushed $(IMG):$(TAG) and removed from local
