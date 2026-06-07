# mcp-ai-studio-web

Public assets and GitHub Pages site for [MCP AI Studio](https://marketplace.visualstudio.com/items?itemName=harishkaparwan.mcp-ai-studio).

Live at: **https://harishkaparwan.github.io/mcp-ai-studio-web/**

## Structure

```
index.html          ← Landing page (served at root)
app/                ← Built React workbench (populated by deploy:web)
public/
  assets/           ← Logo and static images
  policy/
    privacy.html    ← Privacy Policy
.github/workflows/
  deploy.yml        ← GitHub Pages deploy workflow (GitHub Actions)
```

## Deploying the web workbench

From the private `mcp-ai-studio` source repo:

```bash
npm run deploy:web
```

This builds the React app with base `/mcp-ai-studio-web/app/` and copies the output into `mcp-ai-studio-web/app/`. Then commit and push `mcp-ai-studio-web`.
