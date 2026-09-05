# OpenNoiser public integration package

This repository contains public skills and MCP configuration, not the macOS application source.

- Keep names, contact details and authorship under OpenNoiser.
- Use https://opennoiser.com/agents.md and https://opennoiser.com/api/openapi.json as the current integration reference.
- Read prices from the live pricing endpoint; do not hard-code them in skills.
- Preserve read-only tool boundaries. Do not add payment, email, device-control or private-account actions without an explicit product design and authorization model.
- Never include secrets, license keys, customer data, private hostnames, machine identifiers, internal infrastructure details or vendored app dependencies.
- Validate plugin.json and mcp.json against their declared schemas. Keep each skill's frontmatter name and description accurate.
- Public tools require no credentials. Never add a token or cookie to mcp.json.
