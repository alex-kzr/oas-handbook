# SDK evaluation

At the inspected checkpoint the runtime pins `openai-agents` 0.23.1 and Python 3.12. The official SDK tag was verified against its public Git repository. The component lockfile governs the dependency closure. See the [official SDK repository](https://github.com/openai/openai-agents-python) and the [runtime repository](https://github.com/alex-kzr/oas-agents-runtime). A version pin is a reproducibility baseline, not a claim that it is the latest release.

| Capability | Evidence type and conclusion | Limit |
| --- | --- | --- |
| Agent and Runner task contracts | Offline scripted models exercise native control flow and schema checks. | Scripted answers are not genuine model quality. |
| Function tools and approvals | Offline one- and two-gate checkpoint and resume tests exercise bounded native interruptions. | Parallel gates, external exactly-once effects and live checkpoint compatibility remain unverified. |
| Agent tools and handoffs | Scripted manager and handoff coding comparisons use the same controlled sample and validator. | Fixed work does not demonstrate autonomous coding quality or provider cost. |
| MCP | Local synthetic stdio and HTTP integration exercise discovery and selected tool calls. | No real account access or general application authorization is established. |
| Voice and realtime | Scripted or synthetic offline contracts cover selected lifecycle paths. | Live audio quality and full feature coverage remain unverified. |
| Sandbox | Historical controlled container experiments cover finite, provider-free protocols. | They are not a general adversarial isolation guarantee or provider-backed end-to-end proof. |
| Subscription adapter | Separate gated app-server integration has narrowly scoped historical live results. | It does not prove a live native SDK Model/Runner backend. |

OAS application lifecycle, SQLite, consent, observation and adapter code are platform behavior; native SDK Agent, Runner, tools, handoffs and RunState are SDK mechanisms. The offline subscription bridge uses a synthetic injected factory and public SDK interfaces; it does not establish live provider compatibility. A feature status must be tied to its scenario, assertions, mode, revision and limits. Broad SDK inventory, hosted features and native live evaluation remain incomplete; no aggregate completion claim is justified.
