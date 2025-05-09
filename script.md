


# 典型使用场景Tips
## ~~重写tag~~
```bash
docker pull registry.cn-hangzhou.aliyuncs.com/whyym/grafana-image-renderer:latest
docker tag registry.cn-hangzhou.aliyuncs.com/whyym/grafana-image-renderer:latest k8s.gcr.io/grafana-image-renderer/grafana-image-renderer:latest
docker images | grep $(echo k8s.gcr.io/grafana-image-renderer/grafana-image-renderer:latest|awk -F':' '{print $1}')
docker rmi registry.cn-hangzhou.aliyuncs.com/whyym/grafana-image-renderer:latest
```
