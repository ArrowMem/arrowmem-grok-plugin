# ArrowMem for Grok

Security and privacy tools for people running their own local AI models.

## Use it today

This plugin is pending review for the Grok plugin marketplace. You can add it
right now as a custom connector:

1. Go to **grok.com/connectors**
2. Select **New Connector**, then **Custom**
3. Enter the server URL: `https://mcp.arrowmem.ca/mcp`

Grok will discover the available tools and make them usable in conversation.

## What it does

No account or key needed for these:

- **check_ollama_loopback** - checks whether your self-hosted Ollama server is
  reachable from outside your machine, and gives you the complete fix if it is
- **get_privacy_model** - the privacy and security architecture behind ArrowMem
- **get_arrowbridge_info** - running a model on hardware you own, reachable from
  your phone, with no internet in the path
- **get_data_dignity_standard** - an open standard for what a company should tell
  you about your data: what it keeps, who it shares with, which jurisdiction it
  sits in, how you delete it, and what proof you get
- **get_org_info** - what ArrowMem is and who operates it
- **list_packs** - the assistant packs ArrowMem runs

Two further tools, a full Ollama hardening guide and a complete install checker,
require an API key from an ArrowMem subscription.

## About

Built by ArrowMem Inc. https://arrowmem.ca

Licensed under Apache-2.0.
