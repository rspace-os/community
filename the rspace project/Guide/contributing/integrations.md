# Integration Development

RSpace is designed to connect with research tools, services, and infrastructure. There are two fundamentally different ways to build an integration, depending on whether it needs to live inside RSpace or can work entirely from the outside.

## Integrations Inside RSpace

Some integrations are built directly into RSpace — for example, adding a new export target, a new app panel, or a deeper workflow connection. These require changes to the RSpace codebase and follow the standard code contribution process.

If you're considering this kind of integration, reach out first — opensource@researchspace.com or [office hours](../community.md) — so we can discuss the approach and whether it's the right fit.

→ **[Code contributions](code.md)**
→ **[Developer documentation](https://github.com/rspace-os/rspace-web/tree/main/DevDocs)** for architecture and integration patterns


## Integrations Built on/around Public Interfaces

Other integrations don't require touching RSpace code at all. These are built on top of programmatic interfaces that RSpace exposes publicly, and you can develop and publish them entirely independently.

### REST API

The RSpace REST API lets you read and write documents, manage inventory, upload files, search, and export data. Any tool or script that can make HTTP requests can integrate with RSpace this way.

→ **[API Reference](https://community.researchspace.com/public/apiDocs)**
→ Interactive API explorer available on any RSpace instance at `/api/docs`

### Python SDK

The official Python client makes it easy to build scripts, notebooks, and automation tools on top of the API.

→ **[rspace-client-python](https://github.com/rspace-os/rspace-client-python)**

### CLI

A command-line interface for interacting with RSpace from the terminal — useful for scripting, automation, and batch operations.

→ **[rspace-CLI](https://github.com/rspace-os/rspace-cli)** 

### MCP (Model Context Protocol)

MCP servers expose RSpace to AI assistants and LLM-based tools, enabling natural language interaction with research data. An MCP integration can be built in any language and doesn't require any changes to RSpace.

→ **[Example: rspace-mcp](https://github.com/richarda23/rspace-mcp)**
→ **[MCP specification](https://modelcontextprotocol.io)**

MCP is an open protocol — if you build any MCP tools for RSpace, you can publish them independently or add them to our example MCP implementation. 

## Missing API Capabilities?

If you're building an integration and hit a gap in the API, raise an issue on [rspace-web](https://github.com/rspace-os/rspace-web/issues) describing your use case. We prioritise API improvements based on real integration needs.

## Sharing Your Integration

Built something useful? We'd love to help spread the word.

- Email us: opensource@researchspace.com
- Demo it at [office hours](../community.md)
- We can feature it in the newsletter and link to it from the documentation
- Add it to the **[Community Projects](../../community-projects/community-projects.md)** list — open a PR with a short description and your repo link


---
**[contributing ↩](./README.md)** | [home](../../README.md) | [directory](../index.md) | [contact](../contact.md)
