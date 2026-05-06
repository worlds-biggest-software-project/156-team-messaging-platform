# Team Messaging Platform

> Part of the [worlds-biggest-software-project](https://github.com/worlds-biggest-software-project) initiative.
>
> An AI-native, open-source team messaging platform delivering real-time channels, threads, and integrations as a credible alternative to Slack.

Team Messaging Platform is a real-time collaboration tool for engineering teams, SMBs, and security-conscious enterprises that want async messaging without per-seat lock-in or AI features paywalled into top tiers. It combines channel and direct messaging, threaded replies, and a modern integration model with AI capabilities built into the core product rather than reserved for premium plans.

---

## Why Team Messaging Platform?

- **AI features are paywalled by incumbents.** Slack reserves its full Slackbot AI agent and intelligent workspace search for Business+ and Enterprise+ plans, and message search and history are unavailable on the free tier.
- **Per-seat pricing punishes growing teams.** Slack Pro is USD 7.25/user/month and Business+ is USD 12.50/user/month, while Zenzap demonstrates that flat-rate team pricing (~USD 66/month for 50 users vs Slack's ~USD 362.50) is a viable wedge.
- **Microsoft Teams trades simplicity for ecosystem depth.** Teams carries heavy UI complexity and a steep learning curve for non-Microsoft users, optimised more for scheduled meetings than async chat.
- **Google Chat is weak as a standalone messenger.** It depends on Google Workspace and offers limited third-party integrations compared with Slack.
- **Mattermost shows the open-source appetite but leaves AI on the table.** Self-hosted Mattermost gives full data control under MIT licence yet has limited AI features compared to proprietary platforms and significant operational overhead.

---

## Key Features

### Real-Time Messaging Core

- Channel-based and direct messaging with threaded replies
- Real-time bidirectional WebSocket-based message delivery
- File sharing with inline media preview
- User presence indicators, typing indicators, and emoji reactions
- Message persistence, history, and search across channels and DMs

### AI-Native Capabilities

- AI-powered thread and channel summaries and recaps
- AI assistant answering questions via workspace search across messages, files, and linked documents
- Automated action-item extraction from conversations
- Intelligent priority inbox and noise filtering surfacing high-priority messages
- Cross-channel knowledge retrieval across the workspace

### Productivity & Workflow

- Integrated task management with message-to-task conversion (assignee, due date)
- Video calling and screen sharing
- Guest or external user collaboration
- Customisable notification rules
- Administrative dashboard for user and channel management

### Integrations & Extensibility

- OAuth 2.0 authentication with SSO support (SAML 2.0)
- SCIM-based user provisioning for enterprise identity systems
- Slack-compatible webhook integrations for migration
- Connectors for JIRA, GitHub, Salesforce, and other common dev tools
- Web and mobile clients (responsive web/PWA plus native mobile)

### Roadmap Capabilities (backlog)

- Playbooks / workflow automation engine
- Team-health analytics detecting burnout and siloing
- End-to-end encryption option for sensitive conversations
- Decentralised federation (Matrix protocol compatibility)
- Self-hosted deployment option

---

## AI-Native Advantage

Where incumbents tier AI behind premium plans, this project treats AI as core: real-time thread summarisation so teammates can catch up without reading every message; agentic workflow bots that act on natural-language instructions to create tickets, schedule meetings, or update records from a thread; AI-powered noise filtering that separates messages requiring human response from informational and bot traffic; and cross-channel knowledge retrieval that answers questions by searching historical conversations, files, and linked documents. Sentiment and team-health analytics extend AI from convenience into organisational insight, detecting communication breakdowns or decision bottlenecks from interaction patterns.

---

## Tech Stack & Deployment

The platform is designed around real-time WebSocket message delivery (RFC 6455) with OAuth 2.0, SAML 2.0, and OpenID Connect for authentication and SCIM for enterprise user provisioning. A self-hosted deployment option is on the backlog alongside a hosted variant, mirroring the Mattermost pattern of full data residency. Slack-compatible webhook APIs are intended to ease migration. Clients target web (responsive / PWA) and native mobile (iOS, Android).

---

## Market Context

The global team messaging market was valued at USD 8.7 billion in 2024 and is forecast to reach USD 34.2 billion by 2033 at a CAGR of 16.5%; the broader enterprise collaboration software market is estimated at USD 73–86 billion in 2026. Incumbent pricing spans free tiers (Pumble, Slack free) through USD 3–8/user/month mid-market plans (Chanty, Zenzap, Pumble Pro) up to Slack's USD 7.25–12.50/user/month enterprise tiers. Primary buyers are IT and operations leads at SMBs replacing email with async messaging, enterprise CIOs standardising on a collaboration suite, remote-first startups prioritising developer integrations, and security-conscious enterprises requiring self-hosted or private-cloud deployments.

---

## Project Status

> This project is in the **research and specification phase**.  
> Contributions, feedback, and domain expertise are welcome.

---

## Contributing

We welcome contributions from developers, domain experts, and potential users.
See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

**Important:** All contributions must be your own original work or clearly attributed
open-source material with a compatible licence. Copyright infringement and licence
violations will not be tolerated and will result in immediate removal of the offending
contribution. If you are unsure whether a piece of code, text, or other material is
safe to contribute, open an issue and ask before submitting.

---

## Licence

Licence to be determined. See [discussion](#) for context.
