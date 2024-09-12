# graalvm-builder
GraalVM Builder Docker Image

The image can be used in build environment to build Java Native Image.

## Build base Image
### GraalVM CE 22.3.0 ARMx64 builder image - Java 17
```shell
docker buildx build --platform linux/arm64 --build-arg GRAALVM_VERSION=22.3.0 --build-arg JAVA_VERSION=java17 -t alokkusingh/graalvm-ce:22.3.0-java17-arm64 --output=type=docker -f Dockerfile.ol8-java17 .
```
```shell
docker push alokkusingh/graalvm-ce:22.3.0-java17-arm64 
```

#### GraalVM CE 23.1.2 ARMx64 builder image - Java 21
```shell
docker buildx build --platform linux/arm64 --build-arg GRAALVM_VERSION=23.1.2 --build-arg JAVA_VERSION=java21 -t alokkusingh/graalvm-ce:23.1.2-java21-arm64 --output=type=docker -f Dockerfile.ol8-java21 .
```
```shell
docker push alokkusingh/graalvm-ce:23.1.2-java21-arm64 
```