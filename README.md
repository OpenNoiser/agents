# OpenNoiser for agents

Official public agent integrations from [OpenNoiser](https://opennoiser.com). OpenNoiser is a local microphone noise-suppression app for Apple Silicon Macs running macOS 14 or later.

## What this package does

- Check compatibility and build microphone setup checklists.
- Find official troubleshooting and licensing documentation.
- Compare current published plans and renewal terms.

It does not process audio, inspect or change a Mac, access an account, send email or make a payment. This repository does not contain the macOS application or its dependencies.

## Install skills

```sh
npx skills add OpenNoiser/agents
```

Available skills: `opennoiser-setup`, `opennoiser-troubleshooting`, `opennoiser-plans`. See each SKILL.md for when-to-use guidance, workflows and boundaries.

## Connect MCP

| Server | Streamable HTTP endpoint | Tools |
| --- | --- | --- |
| Product | https://opennoiser.com/mcp | get_product, get_pricing, build_setup_checklist |
| Documentation | https://opennoiser.com/mcp/docs | search_docs, get_document |

Both servers are anonymous and read-only. No API key, OAuth setup or customer credentials are required. For Agent Plugins-compatible clients, use the root plugin.json and mcp.json. Hosts supporting MCP Apps can render the pricing tool as an interactive comparison; other hosts receive text and structured data.

## HTTP and browser access

- [Agent instructions](https://opennoiser.com/agents.md)
- [API reference](https://opennoiser.com/api/openapi.json)
- [Authentication](https://opennoiser.com/auth.md)
- [Pricing](https://opennoiser.com/pricing.md)
- [Documentation](https://opennoiser.com/docs/llms.txt)
- [Public resource catalog](https://opennoiser.com/.well-known/ard.json)

WebMCP tools are also registered by the website when the browser supports the API. Markdown twins and Accept: text/markdown are available for content pages.

## Test without payment

POST https://opennoiser.com/api/agent/sandbox/quote with JSON `{"plan":"year","method":"crypto"}`. The result is a synthetic preview: no order, email, account or payment is created. The real checkout determines applicable tax and discounts.

## Support and privacy

[Contact OpenNoiser](https://opennoiser.com/contact) at support@opennoiser.com. Read the [privacy notice](https://opennoiser.com/privacy) and [terms](https://opennoiser.com/terms). Do not include credentials or customer information in issues.

The MIT license applies to this integration package only; it does not license the OpenNoiser macOS app.
