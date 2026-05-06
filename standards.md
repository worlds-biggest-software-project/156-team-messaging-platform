# Standards & API Reference

> Project: Team Messaging Platform · Generated: 2026-05-03

## Industry Standards & Specifications

### ISO Standards

- **ISO/IEC 27001:2022** — Information security management systems; governs the security requirements for team messaging platforms handling confidential business communications; Annex A A.8.11 (Data masking), A.8.12 (Data leakage prevention), and A.8.3 (Information access restriction) are directly applicable. URL: https://www.iso.org/standard/82875.html

- **ISO/IEC 27017:2015 — Cloud Security** — Provides guidelines for information security controls applicable to cloud-delivered messaging services; used by enterprise teams to assess SaaS messaging platform security posture. URL: https://www.iso.org/standard/43757.html

- **ISO/IEC 27018:2019 — Protection of PII in Public Clouds** — Governs processing of employee and user personal data in cloud-hosted messaging platforms; requires data residency transparency and PII handling controls. URL: https://www.iso.org/standard/76559.html

### W3C & IETF Standards

- **RFC 6120 — XMPP Core** — IETF standard defining the Extensible Messaging and Presence Protocol (XMPP); the foundational open protocol for federated instant messaging; used by open-source messaging servers (ejabberd, Prosody) underlying some team chat deployments. URL: https://datatracker.ietf.org/doc/html/rfc6120

- **RFC 6121 — XMPP Instant Messaging** — Extends XMPP Core with instant messaging semantics (contact lists, presence subscriptions, message routing); the IM extension layer used in XMPP-based team chat implementations. URL: https://datatracker.ietf.org/doc/html/rfc6121

- **RFC 7395 — XMPP Subprotocol for WebSocket** — Defines XMPP-over-WebSocket binding enabling real-time bidirectional messaging in browsers without long-polling; relevant to web client implementation. URL: https://www.rfc-editor.org/rfc/rfc7395.html

- **RFC 6455 — WebSocket Protocol** — W3C/IETF standard for full-duplex real-time communication over a single TCP connection; used by all major team messaging platforms for real-time message delivery (Slack, Discord, Mattermost, Zulip). URL: https://datatracker.ietf.org/doc/html/rfc6455

- **RFC 7519 — JSON Web Token (JWT)** — Standard token format used for authenticating API requests and bot/app tokens in team messaging platforms. URL: https://datatracker.ietf.org/doc/html/rfc7519

- **RFC 6749 — OAuth 2.0** — Authorization framework used by all major team messaging platforms for bot and app authentication, Slack app distribution, and third-party integration authorization flows. URL: https://datatracker.ietf.org/doc/html/rfc6749

- **RFC 7231 — HTTP/1.1 Semantics** — Underpins all REST API management interfaces used by team messaging platforms for programmatic message sending, channel management, and user administration. URL: https://datatracker.ietf.org/doc/html/rfc7231

### Data Model & API Specifications

- **Matrix Specification (v1.17, 2025)** — Open standard protocol for decentralised, federated real-time communication; defines Client-Server API, Federation API, Application Service API, and Identity Service API; natively supports end-to-end encryption (Olm/Megolm), room-based messaging, persistent history, and voice/video (MatrixRTC); adopted by 10+ national governments as of 2025. URL: https://spec.matrix.org/latest/

- **Matrix Client-Server API** — The primary API for Matrix clients; REST/JSON-based; supports room creation, message sending (m.room.message events), presence, read receipts, push notifications, and VoIP signalling. URL: https://spec.matrix.org/latest/client-server-api/

- **OpenAPI 3.1** — Used by Slack, Discord, and Mattermost to describe their REST management APIs; enables SDK generation, Postman collections, and CI/CD pipeline integration. URL: https://spec.openapis.org/oas/latest.html

- **JSON:API Specification** — HackerOne's REST API compliance standard; Slack's APIs return JSON:API-compatible structures for consistent pagination, filtering, and relationship traversal. URL: https://jsonapi.org/

- **WebRTC** — W3C standard for browser-based real-time audio/video communication; used in in-platform huddle/call features (Slack Huddles, Mattermost Calls, Element Call via MatrixRTC). URL: https://www.w3.org/TR/webrtc/

### Security & Authentication Standards

- **GDPR Article 6 & 32 — Lawful Processing and Security of Processing** — Team messaging platforms handling EU employee communications must maintain lawful basis for processing, offer configurable retention policies, and implement appropriate technical security measures; data residency in EU/EEA is the simplest compliance path. URL: https://gdpr-info.eu/art-32-gdpr/

- **EU AI Act (2024/2847) — Title III** — AI systems embedded in team messaging platforms (AI summarisation, automated triage, AI agents) that affect employees are subject to transparency and human oversight requirements under the EU AI Act (enforcement from August 2025 for GPAI models). URL: https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024R2847

- **SOC 2 Type II** — De facto enterprise compliance standard for SaaS messaging platforms; required by large enterprise customers for procurement; covers Security, Availability, Confidentiality, Processing Integrity, and Privacy trust service criteria. URL: https://www.aicpa-cima.com/topic/audit-assurance/audit-and-assurance-greater-than-soc-2

- **NIST SP 800-63B — Digital Identity Guidelines: Authentication** — Governs authentication assurance levels for team messaging platform login; enterprise deployments typically require AAL2 (phishing-resistant MFA) for access. URL: https://csrc.nist.gov/publications/detail/sp/800-63b/4/draft

- **OWASP API Security Top 10 (2023)** — Governs the design of team messaging REST APIs and bot/app integration security; API2 (Broken Authentication) and API1 (Broken Object Level Authorization) are particularly relevant to channel and DM access control. URL: https://owasp.org/API-Security/

- **CCPA/CPRA — California Consumer Privacy Act** — Team messaging platforms serving California employees or users must provide data deletion rights, opt-out of sale, and data access on request; impacts message retention and export design. URL: https://oag.ca.gov/privacy/ccpa

### MCP Server Specifications

Team messaging platforms are central to the 2025-2026 MCP ecosystem:

- **Slack MCP Server (Official, October 2025)** — Slack's official MCP server allows external AI clients (Claude, Perplexity, others) to search messages, retrieve channel content, send messages, manage canvases, and manage users within a Slack workspace. MCP tool calls and Real-Time Search queries grew 25x between October 2025 and March 2026. URL: https://docs.slack.dev/ai/slack-mcp-server/

- **@modelcontextprotocol/server-slack (npm)** — Official Anthropic/MCP community Slack MCP server package; open-source reference implementation for Slack workspace access via MCP. URL: https://www.npmjs.com/package/@modelcontextprotocol/server-slack

- **Slack as Agentic OS (2026)** — Slack has repositioned itself as an "agentic operating system" with both MCP server (external AI clients access Slack) and MCP client (Slackbot reaches into external MCP tools from within conversations) capabilities; 50+ AI partners building agents on the platform as of April 2026. URL: https://slack.com/blog/news/powering-agentic-collaboration

---

## Similar Products — Developer Documentation & APIs

### Slack

- **Description:** Dominant commercial team messaging platform; channel-based, threaded messaging; 20M+ daily active users; deep integration ecosystem with 2,400+ apps; evolving into an agentic platform with MCP server/client duality (October 2025).
- **API Documentation:** https://docs.slack.dev/apis/ and https://api.slack.com/methods
- **OpenAPI Specs:** https://github.com/slackapi/slack-api-specs
- **SDKs/Libraries:** Bolt SDK (JavaScript/Python/Java); Python slack_sdk; Go slack-go; Java slack-api-client
- **Developer Guide:** https://docs.slack.dev/
- **Standards:** REST/JSON, WebSocket (Real-Time Messaging API), OAuth 2.0, OpenAPI 3.1
- **Authentication:** OAuth 2.0 (app installation); Bot tokens; User tokens; App-level tokens for Socket Mode

### Microsoft Teams (Microsoft Graph API)

- **Description:** Enterprise team messaging integrated into Microsoft 365; strongest in regulated industries and Microsoft-heavy IT environments; 320M+ daily active users; accessible programmatically via Microsoft Graph API.
- **API Documentation:** https://learn.microsoft.com/en-us/graph/api/resources/teams-api-overview
- **SDKs/Libraries:** Microsoft Graph SDKs (Python, .NET, Go, Java, JavaScript/TypeScript); Teams SDK (@microsoft/teams.graph); Graph Explorer web tool
- **Developer Guide:** https://developer.microsoft.com/en-us/graph
- **Standards:** REST/JSON, OpenAPI 3.1, OAuth 2.0 (Azure AD), WebSocket (Teams Toolkit)
- **Authentication:** Azure AD OAuth 2.0 (delegated or application permissions); managed identity for Azure workloads

### Discord

- **Description:** Originally gaming-focused, now widely adopted by developer communities and open-source projects; channel/server model with threads; 70% of new OSS projects default to Discord for community engagement (2026); strong bot ecosystem.
- **API Documentation:** https://discord.com/developers/docs/
- **SDKs/Libraries:** discord.js (JavaScript); discord.py (Python); JDA (Java); DSharpPlus (.NET); discord-go (Go)
- **Developer Guide:** https://discord.com/developers/docs/getting-started
- **Standards:** REST/JSON, WebSocket Gateway (real-time events), OAuth 2.0, OpenAPI
- **Authentication:** Bot token (Authorization: Bot {token}); OAuth 2.0 for user applications

### Matrix / Element (Open Standard)

- **Description:** Open-source, decentralised, federated team messaging protocol (Matrix) with reference server (Synapse/Dendrite) and client (Element); adopted by 10+ national governments; end-to-end encrypted by default; MatrixRTC for voice/video; Matrix v1.17 current spec as of late 2025.
- **API Documentation:** https://spec.matrix.org/latest/client-server-api/
- **SDKs/Libraries:** matrix-js-sdk (JavaScript); matrix-rust-sdk (Rust); matrix-nio (Python); matrix-android-sdk2; matrix-ios-sdk
- **Developer Guide:** https://matrix.org/docs/develop/
- **Standards:** Matrix Client-Server API (REST/JSON), Federation API, WebSocket-based sync, Olm/Megolm E2EE, MatrixRTC (WebRTC-based)
- **Authentication:** Access token (bearer); OAuth 2.0 (Matrix 1.7+ OIDC login); homeserver registration

### Mattermost (Open Source)

- **Description:** Open-source (MIT-licensed) self-hosted team messaging platform; DevOps-focused; strong in regulated industries requiring on-premises data residency; integrates with developer tools (GitHub, Jira, GitLab); REST and WebSocket APIs.
- **API Documentation:** https://api.mattermost.com/
- **SDKs/Libraries:** mattermost-client (JavaScript); mattermost4j (Java); mattermost-go (Go); Python mattermostautodriver
- **Developer Guide:** https://developers.mattermost.com/
- **Standards:** REST/JSON, WebSocket, OpenAPI 3.0, OAuth 2.0, SAML 2.0, LDAP
- **Authentication:** Bearer token (personal access tokens or session tokens); OAuth 2.0 for apps; SAML 2.0 for enterprise SSO

### Rocket.Chat (Open Source)

- **Description:** Open-source (MIT-licensed) omnichannel messaging platform; internal team chat plus customer-facing live chat, social media integration, and contact centre; strong customisation and white-label options; REST and Realtime (WebSocket) APIs.
- **API Documentation:** https://developer.rocket.chat/
- **SDKs/Libraries:** Rocket.Chat JS SDK; Python Rocket.Chat SDK; Rocket.Chat Apps SDK (TypeScript)
- **Developer Guide:** https://developer.rocket.chat/
- **Standards:** REST/JSON, WebSocket Realtime API (DDP protocol), OAuth 2.0, SAML 2.0, LDAP, OpenAPI
- **Authentication:** Auth token + user ID (session-based); OAuth 2.0; personal access tokens

### Zulip (Open Source)

- **Description:** Open-source (Apache 2.0) team messaging with unique topic-based threading model; streams (channels) + topics provide persistent, searchable conversation organisation; used by major open-source communities; REST API and webhook integrations.
- **API Documentation:** https://zulip.com/api/
- **SDKs/Libraries:** python-zulip-api (official Python); zulip-js (JavaScript); zulip-rs (Rust); matterbridge supports Zulip
- **Developer Guide:** https://zulip.com/api/
- **Standards:** REST/JSON, OpenAPI, WebSocket (event queue), OAuth 2.0, SAML 2.0, LDAP
- **Authentication:** API key (email + key pair for bots and integrations); OAuth 2.0 for external apps

### Matterbridge (Open Source)

- **Description:** Open-source (Apache 2.0) bridge connecting 20+ messaging platforms including Slack, Discord, Teams, Matrix, Mattermost, Rocket.Chat, Zulip, XMPP, IRC, Telegram, and WhatsApp; REST API for cross-platform message routing.
- **API Documentation:** https://github.com/42wim/matterbridge/wiki
- **SDKs/Libraries:** Go library; REST API bridge configuration
- **Developer Guide:** https://github.com/42wim/matterbridge
- **Standards:** Abstracts over each connected platform's native API/protocol; REST/JSON for management
- **Authentication:** Per-platform credentials configured in TOML; token-based for API-enabled platforms

---

## Notes

- **Matrix gaining government adoption (2025-2026)**: Matrix saw 10+ national governments join the 2025 Matrix Conference; The Register reported in February 2026 that Matrix/Element is gaining significant ground in government IT as a sovereign, self-hosted alternative to Slack and Teams. Matrix v1.17 and MatrixRTC for multi-user video represent the protocol's maturation.

- **Slack as agentic OS (2026)**: Slack's launch of its official MCP server in October 2025 and its 25x growth in MCP tool calls by March 2026 represents a fundamental shift — team messaging platforms are becoming the AI agent coordination layer for enterprise workflows.

- **Classic app deprecation (Slack, May 2026)**: Slack's classic app API (legacy bot tokens, RTM API) is deprecated as of May 25, 2026; all integrations must migrate to Bolt SDK + Events API + Socket Mode.

- **XMPP still relevant**: Despite being a 2004 standard, XMPP (RFC 6120/6121) remains actively maintained and is used in enterprise deployments where federation and open standards are required; ejabberd and Prosody are production-grade open-source servers.

- **Data residency as enterprise requirement**: The convergence of GDPR, EU AI Act, and DORA requirements is driving enterprise customers to require EU data residency for messaging platforms; self-hosted Matrix, Mattermost, and Rocket.Chat are the primary beneficiaries.
