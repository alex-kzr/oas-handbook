# OAS Handbook

OpenAI Agents Platform (OAS) is a Python-centered foundation for reusable agent tasks and for evaluating the OpenAI Agents SDK. It separates application task execution from reproducible SDK experiments and provides an operator console, synthetic integration fixtures, and retained evidence. It is a distinct project with its own boundaries.

This handbook is for developers and architects evaluating the platform. It describes an inspected local checkpoint, not a claim that every described change is published.

## Contents

- [Overview](https://github.com/alex-kzr/oas-handbook/blob/master/docs/overview.md) — purpose and boundaries.
- [Architecture](https://github.com/alex-kzr/oas-handbook/blob/master/docs/architecture.md) — components, ownership and data flow.
- [Repository catalog](https://github.com/alex-kzr/oas-handbook/blob/master/docs/repositories.md) — component repositories and source availability.
- [Workflows](https://github.com/alex-kzr/oas-handbook/blob/master/docs/workflows.md) — task execution, approvals and observation.
- [SDK evaluation](https://github.com/alex-kzr/oas-handbook/blob/master/docs/sdk-evaluation.md) — evidence by capability and mode.
- [Integrations](https://github.com/alex-kzr/oas-handbook/blob/master/docs/integrations.md) — subscription adapter, MCP, sample service and sandbox.
- [Development and operations](https://github.com/alex-kzr/oas-handbook/blob/master/docs/development.md) — prerequisites, offline checks and diagnostics.
- [Glossary](https://github.com/alex-kzr/oas-handbook/blob/master/docs/glossary.md) — platform terminology.

The current platform is a local, single-operator foundation, not a production multi-user service. Offline scripted results, local integration results, and narrowly authorized live observations have different evidentiary value.
