# Minikube

I. Create cluster

```shell
minikube start --cpus 2 --memory 4g --driver docker --profile polar
```
II. Use cluster

```shell
minikube profile polar
```

III. Create namespace

```shell
kubectl create namespace polar
```
III. Sync docker

```shell
eval $(minikube -p minikube docker-env)
```

# Gradle

I. Build

```shell
gradle clean build -x test
```
II. Image
```shell
gradle bootBuildImage
```