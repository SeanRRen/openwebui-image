## Download
```shell
docker pull ghcr.io/open-webui/open-webui:ollama
```

## Start
```shell
# Create Folder
cd /root
mkdir ollama open-webui

# Run
docker run -d -p 3000:8080 -v /root/ollama:/root/.ollama -v /root/open-webui:/app/backend/data --name open-webui --restart always ghcr.io/open-webui/open-webui:ollama
```
