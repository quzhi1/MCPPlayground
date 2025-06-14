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

## Gradio server
### Installation
```bash
pip install "gradio[mcp]"
```

### Run server
```bash
python gradio-server.py
```