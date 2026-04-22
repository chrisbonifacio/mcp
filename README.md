# 🌟 Microsoft MCP Servers


## 📘 What is MCP?

**Model Context Protocol (MCP)** is an open protocol that standardizes how applications provide context to large language models (LLMs).

## 📚 Which MCP Servers are available from Microsoft?

### Azure
- **INSTALL**: [![Install Azure MCP in VS Code](https://img.shields.io/badge/VS_Code-0098FF?style=flat-square&logo=visualstudiocode&logoColor=white)](https://vscode.dev/redirect?url=vscode:extension/ms-azuretools.vscode-azure-mcp-server) [![Add to Kiro](https://kiro.dev/images/add-to-kiro.svg)](https://kiro.dev/launch/mcp/add?name=azure-mcp-server&config=%7B%22command%22%3A%22npx%22%2C%22args%22%3A%5B%22-y%22%2C%22%40azure%2Fmcp%40latest%22%2C%22server%22%2C%22start%22%5D%7D)

### Microsoft Fabric (Public Preview)
- **INSTALL**: [microsoft/mcp](https://github.com/microsoft/mcp/tree/main/servers/Fabric.Mcp.Server#readme) [![Add to Kiro](https://kiro.dev/images/add-to-kiro.svg)](https://kiro.dev/launch/mcp/add?name=fabric-mcp-server&config=%7B%22command%22%3A%22npx%22%2C%22args%22%3A%5B%22-y%22%2C%22%40microsoft%2Ffabric-mcp%40latest%22%2C%22server%22%2C%22start%22%2C%22--mode%22%2C%22all%22%5D%7D)

## Install in Kiro

Manual install: Open `.kiro/settings/mcp.json` or `~/.kiro/settings/mcp.json` and add:

```json
"azure-mcp-server": {
  "command": "npx",
  "args": ["-y", "@azure/mcp@latest", "server", "start"]
}
```

```json
"fabric-mcp-server": {
  "command": "npx",
  "args": ["-y", "@microsoft/fabric-mcp@latest", "server", "start", "--mode", "all"]
}
```
