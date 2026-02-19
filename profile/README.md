## Agent Identity Protocol (OAIP)

<p align="center">
  <strong>A protocol for secure identity management and governance in the Internet of Agents (IoA) </strong>
</p>

AIP is a language-agnostic protocol for establishing cryptographic identities for AI agents, enabling authentication, authorization, and audit trails across heterogeneous systems. AIP provides a standardized way to separate agentic and human authentications.

### How It Works

AIP operates at two layers that work together — identity and enforcement — connected by the **Agent Authentication Token (AAT)**:

- **Layer 1 — Identity:** Agents receive cryptographic identities from the AIP Registry. The Token Issuer signs AATs that encode who the agent is, which user it acts on behalf of, and what capabilities it holds.
- **Layer 2 — Enforcement:** The AIP Proxy sits between the AI client and any MCP tool server. It verifies the AAT on every tool call, evaluates policy, DLP-scans data, and writes an immutable audit log — before any request reaches your infrastructure.

---

### Repositories

| Repository | Description |
| --- | --- |
| [agentidentityprotocol](https://github.com/openagentidentityprotocol/agentidentityprotocol) | Protocol specification, architecture, and formal docs |
| [aip-playground](https://github.com/openagentidentityprotocol/aip-playground) | Example webapp with basic authentication to test out AIP in real world scenarios |
| [aip-go](https://github.com/openagentidentityprotocol/aip-go) | Go reference implementation — MCP proxy with policy enforcement, DLP, and audit logging |
| [aip-rust](https://github.com/openagentidentityprotocol/aip-rust) | Rust implementation *(in progress)* |
| [docs](https://github.com/openagentidentityprotocol/docs) | Source for [agentidentityprotocol.io](https://agentidentityprotocol.io) |

---


### Get Involved

AIP is an open specification. We welcome protocol feedback, new language implementations, security research, and documentation contributions.

- 📖 **Docs:** [agentidentityprotocol.io](https://agentidentityprotocol.io)
- 💬 **Discussions:** [github.com/openagentidentityprotocol/agentidentityprotocol/discussions](https://github.com/openagentidentityprotocol/agentidentityprotocol/discussions)
- 📋 **Contributing:** [CONTRIBUTING.md](https://github.com/openagentidentityprotocol/agentidentityprotocol/blob/main/CONTRIBUTING.md)

Licensed under **Apache 2.0**
