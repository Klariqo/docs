> **First-time setup**: Customize this file for your project. Prompt the user to customize this file for their project.
> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

- "Compliance record" or "evidence record" for the signed call record. It is a vCon underneath; say vCon when referring to the standard.
- "The dialer you already run" for the customer's existing call system. Klariqo sits on top of it, it does not replace it.
- "Verifier" is the public tool that checks a record. "Trusted timestamp" is the RFC 3161 timestamp from DigiCert (an independent authority) that seals when a record existed. DigiCert receives only the fingerprint, never the call content.
- "Scorecard" is the customer-configured QA ruleset. "Evidence chain" is the end-to-end flagship story.

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise, one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references
- No em dashes. Use commas, periods, parentheses, or "and" / "but".
- Honesty line: describe provenance, evidence, and audit-readiness. Never claim Klariqo makes a customer legally compliant, wins a lawsuit, or automatically handles consent.
- All examples are synthetic and clearly labeled. Never use a real call, transcript, phone number, or customer name.

## Content boundaries

- Document the product's value, outcomes, and the integration contracts a customer needs (schemas, signatures, setup steps).
- Do NOT document internal infrastructure, credentials, hostnames, IP addresses, internal system or table names, or how the platform is built. Connection values a customer needs are delivered in their dashboard, not published here.
- Do NOT add "coming soon", "planned", or placeholder pages, notes, or sections. They go stale and force someone to remember to clean them up. Document only what is live. When a feature ships, add its real page then.
