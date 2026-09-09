# ArrowMem for Grok

Security and privacy tools for people running local AI models and MCP agents.

## Use it today

This plugin is pending review for the Grok plugin marketplace. You can add it
right now as a custom connector:

1. Go to **grok.com/connectors**
2. Select **New Connector**, then **Custom**
3. Enter the server URL: `https://mcp.arrowmem.ca/mcp`

Grok will discover the available tools and make them usable in conversation.

## How it works

**These tools never reach your machine.** Grok runs the diagnostic commands
locally and passes their output in as arguments. Nothing you submit is stored,
logged or retained, and each call is evaluated on its own.

Every check returns **pass**, **fail**, or **unverifiable**. If you did not
supply the data a check needs, it says so and tells you the command to run. It
never reports a pass it did not verify.

## What it does

No account or key needed for these:

- **inventory_ai_agents** - lists every MCP server configured on your machine
  (Claude Desktop, Claude Code, Cursor) and every tool each one exposes, with a
  hash per tool, so you can tell when a tool you already approved changes what
  it does. Hosts that keep their configuration in your provider account rather
  than on your machine cannot be read locally by anyone, and it names those as
  unchecked rather than leaving them out of the report
- **check_ollama_loopback** - checks whether your Ollama install is reachable
  from your network or bound to your own machine only
- **check_ollama_hardening** - the fuller check: bind address, the reverse proxy
  and its configuration, disk encryption
- **get_hardening_guide** - the complete, live-tested procedure for hardening a
  self-hosted Ollama server
- **get_privacy_model** - the privacy and security architecture behind ArrowMem
- **get_arrowbridge_info** - running a model on hardware you own, reachable from
  your phone, with no internet in the path
- **get_data_dignity_standard** - an open standard for what a company should tell
  you about your data: what it keeps, who it shares with, which jurisdiction it
  sits in, how you delete it, and what proof you get
- **get_org_info** - what ArrowMem is and who operates it
- **list_packs** - the assistant packs ArrowMem runs

Two tools need an API key, and are not part of this free listing:

- **check_exposed_services** - the whole-machine sweep: Postgres, MongoDB, Redis,
  Elasticsearch, Jupyter and Ollama, plus firewall state, disk encryption, screen
  lock and pending updates
- **enrol_alert_relay** - enrols an ArrowMem key in the Guard alert relay: a
  watchdog topic and a one-time family link a trusted person can use to check
  on you if a call sounds like you and asks for money

## About

Built by ArrowMem Inc. https://arrowmem.ca

Licensed under Apache-2.0.
