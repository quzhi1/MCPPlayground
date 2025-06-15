# MCPPlayground
This is my playground for building MCP server and applications

## Python MCP server
### Installation
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
cd python
pip install -r requirements.txt
```

### Run server
```bash
cd python
mcp dev server.py
```
MCP server should be available by browser with http://127.0.0.1:6274/?MCP_PROXY_AUTH_TOKEN=...
Just click the link in your server log.

## MCP client
### Installation
```bash
npm install -g npx
pip install "huggingface_hub[mcp]>=0.32.0"
huggingface-cli login
```

## Simple Gradio server
### Installation
```bash
pip install "gradio[mcp]"
```

### Run server
```bash
python gradio-server.py
```

## Sentiment analysis server
### Installation
```bash
source .venv/bin/activate
cd python
pip install "gradio[mcp]" textblob
```

### Run server
```bash
python app.py
```
Some useful URLs:
1. UI: http://localhost:7860
2. MCP server (SSE): http://127.0.0.1:7860/gradio_api/mcp/sse
3. MCP schema: http://localhost:7860/gradio_api/mcp/schema