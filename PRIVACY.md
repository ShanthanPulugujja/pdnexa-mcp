# Privacy

pdnexa PDF is a free plugin package. It points Cursor or Grok Bot at the pdnexa MCP server. This repository does not collect data and does not contain account secrets.

## What the MCP server handles

When you use a PDF tool, the client sends the PDF to:

`https://adr-mcp.vercel.app/mcp`

Processing is **server-ephemeral**:

- PDFs are processed on the pdnexa MCP server for that job.
- Output files are kept for about **30 minutes**, then deleted.
- Download URLs stop working on that same window.
- MCP does not keep a durable PDF library.

`mcp_quota` reads the account meter for the current UTC month. It does not upload a PDF.

## Account

Authorization uses an existing pdnexa account. Google sign-in does not auto-create a pdnexa account. Job metering (3 completed jobs per UTC month on free accounts) is tied to that account.

## What this listing does not do

- It does not sell access, subscriptions, or extra jobs.
- Paid uncapping is offered only at [https://pdnexa.com](https://pdnexa.com).
- This git repo does not store your PDFs, tokens, or client credentials.

Questions: see [SUPPORT.md](SUPPORT.md).
