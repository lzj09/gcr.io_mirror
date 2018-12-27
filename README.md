# gcr.io_mirror
gcr.io镜像

## tiller:v2.12.1
由于网络的原因，如果直接：
```java
docker pull gcr.io/kubernetes-helm/tiller:v2.12.1
```
可能会下载失败。

解决办法是：
执行下如下命令：
```java
docker pull lzj09/tiller:v2.12.1
docker tag lzj09/tiller:v2.12.1 gcr.io/kubernetes-helm/tiller:v2.12.1
```
