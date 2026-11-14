<p align="center"><img src="assets/logo-256.png" width="64" alt="Tributs"></p>

# Tributs MCP

Connect your AI assistant to [Tributs](https://tributs.ad/en/ai), the accounting and tax software built for Andorra, and ask about your company in plain language.

**Server URL:** `https://mcp.tributs.ad/mcp` · Streamable HTTP · OAuth (sign in with your Tributs account) · **read-only**

## What you can ask

- **Invoices:** what's unpaid or overdue, who owes you and how much, what you owe suppliers.
- **Bank:** account balances and transactions.
- **Tax:** upcoming and overdue obligations (IGI, corporate tax, non-resident tax, CASS) with the figures of each filing.
- **Accounting:** chart of accounts, journal lines, trial balance, profit and loss, balance sheet.
- **Payroll:** employees, payslips and monthly totals.
- **Accounting firms:** one question across every client company you manage.

Examples:

> Which sales invoices are overdue, and how much do customers owe me in total?
> What tax filings do I have due in the next 30 days?
> Show my profit and loss for this year compared with last year.

The connector cannot create, change or delete anything. It only sees the companies your Tributs user can already see, and you can revoke access at any time in Tributs → Profile → External connections.

## Install

| Assistant | How |
|---|---|
| **Claude** | Settings → Connectors → Add custom connector → `https://mcp.tributs.ad/mcp` |
| **ChatGPT** | Settings → Apps → add `https://mcp.tributs.ad/mcp` |
| **Cursor** | [Add to Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=Tributs&config=eyJ1cmwiOiJodHRwczovL21jcC50cmlidXRzLmFkL21jcCJ9), or install this repository as a plugin |
| **VS Code** | Command palette → *MCP: Add Server* → HTTP → `https://mcp.tributs.ad/mcp` |
| **Grok** | grok.com/connectors → New Connector → Custom → `https://mcp.tributs.ad/mcp` |
| **Other clients** | Any MCP client that supports remote servers with OAuth |

Prefer an API key? Create a personal token in Tributs → Profile → External connections and send it as `Authorization: Bearer trb_…`.

## Links

- Website: https://tributs.ad/en/ai
- API docs: https://tributs.ad/developers
- Privacy: https://tributs.ad/legal/privacy · Terms: https://tributs.ad/legal/terms
- Support: hola@tributs.ad
- MCP Registry: `ad.tributs/mcp`

This repository contains only the connector manifest; the server is operated by Alastia. Tributs is a private product and is not an official service of the Government of Andorra.
