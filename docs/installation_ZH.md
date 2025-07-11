## 下载镜像
```shell
docker pull ghcr.io/open-webui/open-webui:ollama
```

## 启动
```shell
# 创建主机目录
cd /root
mkdir ollama open-webui

# 运行
docker run -d -p 3000:8080 -v /root/ollama:/root/.ollama -v /root/open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:ollama

```