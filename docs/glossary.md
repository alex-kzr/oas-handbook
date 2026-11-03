# Glossary

- **OAS:** OpenAI Agents Platform, the umbrella and its independently maintained components.
- **Task definition:** Versioned application contract and execution strategy for a reusable task type.
- **TaskRun:** Persisted application record for one task execution, distinct from an SDK session or RunState.
- **Scenario:** Reproducible SDK capability experiment with explicit prerequisites and assertions.
- **Approval:** A recorded decision permitting a particular bounded action or continuation; it is not general permission for unrelated requests.
- **RunState:** SDK execution state used by supported interruption and resume paths; platform persistence and replay safety remain separate concerns.
- **MCP:** Model Context Protocol, used here with a synthetic local server fixture.
- **Offline:** A test mode using scripted or synthetic behavior without a live provider request.
- **Integration:** A test across a real local component or protocol boundary; it does not by itself establish live provider behavior.
- **Live:** An actual authorized provider or subscription interaction, scoped to its specific request and recorded observation.
- **Subscription adapter:** OAS integration with a Codex app server, distinct from a proven live native SDK Model backend.
