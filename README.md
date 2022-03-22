# docker-zeppelin

Apache Zeppelin build from official Dockerfile with support for both AMD64 and ARM64 architectures.

Usage:
```
docker run -it --rm -p 7077:7077 -p 8080:8080 \
--privileged=true \
-v $PWD/logs:/logs \
-v $PWD/notebook:/notebook \
-v /local/path/to/data:/data \
-e ZEPPELIN_NOTEBOOK_DIR='/notebook' \
-e ZEPPELIN_LOG_DIR='/logs' \
snilard/zeppelin:0.10.0
```

Github repository: https://github.com/snilard/docker-zeppelin