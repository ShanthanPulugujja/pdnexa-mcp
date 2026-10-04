# pdnexa PDF

Cursor and Grok Bot plugin for the [pdnexa](https://pdnexa.com) PDF MCP server.

The plugin is **free to install**. It does not sell a subscription, seat, or job pack through the Cursor Marketplace or Grok Bot Plugins. Paid uncapping stays on [pdnexa.com](https://pdnexa.com) only.

## What it does

Remote MCP endpoint (no secrets in this repo):

`https://adr-mcp.vercel.app/mcp`

Tools:

| Tool | What it does |
| --- | --- |
| `pdf_merge` | Merge two or more PDFs into one PDF. |
| `pdf_split` | Split one PDF by 1-based inclusive page ranges. |
| `pdf_extract_pages` | Extract specific 1-based pages into a new PDF. |
| `pdf_rotate` | Rotate pages by 90, 180, or 270 degrees. |
| `pdf_compress` | Rewrite a PDF with compressed object streams. |
| `mcp_quota` | Show this account’s MCP meter for the current UTC month. Does not upload a PDF and does not use a job. |
| `mcp_job_status` | Look up a job and its download URLs. |

Completed jobs return download URLs. **Output files are ephemeral and stop working about 30 minutes after the job is created.** pdnexa MCP does not keep a durable PDF library.

## Install

After this plugin is listed:

- **Cursor:** open the Cursor Marketplace and install **pdnexa PDF**.
- **Grok Bot:** open Plugins and install **pdnexa PDF**.

You can also load this public repository as a Cursor plugin (`mcp.json` is discovered from the repo root).

## Authorize

You need an **existing pdnexa account**. Signing in with Google does **not** create a pdnexa account for you.

1. Install the plugin.
2. Connect the `pdnexa` MCP server.
3. Authorize with the pdnexa account you already have.

This package has no API keys, client IDs, or other secrets. Do not add any.

## Free meter

Free accounts can complete **3 jobs per UTC month**.

- Only a **completed** job counts.
- `mcp_quota` does not count.
- The month boundary is **UTC**, not local time.
- An active paid entitlement is uncapped. Buy or manage that on [https://pdnexa.com](https://pdnexa.com) only. This Marketplace / Plugins listing does not take payment.

## Privacy and support

- [PRIVACY.md](PRIVACY.md)
- [SECURITY.md](SECURITY.md)
- [SUPPORT.md](SUPPORT.md)
- [LICENSE](LICENSE) (MIT)
