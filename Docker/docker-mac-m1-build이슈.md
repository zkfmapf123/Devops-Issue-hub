# Docker MAC M1 Build시 Platform 이슈

![1](../public/1.png)

## 해결법

```sh
## linux/amd64 꼭 붙혀라...
docker build -t zkfmapf123/node-fluentd:5.0 --platform linux/amd64 . && docker push zkfmapf123/node-fluentd:5.0  
```
