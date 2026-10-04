# Security

## Reporting a vulnerability

Please report a security issue in this plugin package or the pdnexa MCP endpoint privately through [pdnexa.com](https://pdnexa.com) support rather than in a public GitHub issue. Include steps to reproduce and the affected URL or file. Do not include live tokens, session cookies, or full customer PDFs.

## Scope of this repository

This repository is packaging only:

- Plugin manifest (`.cursor-plugin/plugin.json`)
- MCP client config (`mcp.json`) with the public URL `https://adr-mcp.vercel.app/mcp`
- Docs and logo

There are **no secrets**, static client IDs, or credentials in the tree. Do not commit any.

## Operational notes

- Use the URL above. `mcp.pdnexa.com` is not the MCP host for this plugin.
- Treat job download URLs as short-lived (about 30 minutes).
- Authorize only with an existing pdnexa account you control.
