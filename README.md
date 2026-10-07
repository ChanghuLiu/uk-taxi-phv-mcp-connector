# UK Taxi PHV Licensing

Public connector metadata for the hosted **UK Taxi PHV Licensing** MCP service operated by RegEvidenceHub.

## Remote MCP

`https://taxi.regevidencehub.com/mcp`

This repository intentionally contains only public installation and service-discovery metadata. The hosted service implementation is maintained separately.

## What it does

Evidence-linked taxi and private-hire licensing preflight and local-authority comparison for England.

## Installation

Use the remote MCP endpoint above, or import the included `.mcp.json` in clients that support MCP configuration files.

## Payment

Agent-native paid MCP actions use x402 where payment is required. Human-facing premium checkout remains available separately through RegEvidenceHub.

## Publisher

RegEvidenceHub — https://www.regevidencehub.com/


## Gemini CLI

Install this connector as a Gemini CLI extension:

```sh
gemini extensions install https://github.com/ChanghuLiu/uk-taxi-phv-mcp-connector
```

The Gemini CLI extension connects to the hosted Streamable HTTP MCP endpoint above. Gemini CLI does not automatically sign x402 payments; paid tools may return a payment-required response and need a separate x402-capable payment workflow. Do not put wallet private keys in this extension.
