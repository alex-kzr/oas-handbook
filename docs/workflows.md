# Workflows

## Tasks and approval

A registered task definition supplies a versioned input/output contract, execution strategy and controls. The runtime validates input, records a TaskRun and executes the selected strategy. Task and SDK scenario registries have separate identities and purposes. Scripted technical briefs and sample review tasks exercise contracts without claiming model quality. Sample review uses a disposable copy of the controlled target.

The application can persist a pending approval and pause. In the tested bounded native-tool checkpoint path, a decision is bound to the task and state version; approval makes the run ready and explicit resume continues it. One or two sequential synthetic gates and separate-process restore have been tested. Duplicate decisions and consumed checkpoints are guarded. Arbitrary parallel gates, authenticated decision makers and external exactly-once effects are not established by these fixtures.

The runtime records status, events, result references and available correlations. Cooperative local ownership prevents tested duplicate execution; uncertain interrupted work is marked as such rather than automatically replayed. Cancellation and recovery depend on the task strategy. An unknown remote outcome is not proof of remote cancellation or a refunded charge.

## CLI, API and observation

The CLI exposes catalog, scenario and task operations. The console talks to the versioned local API, including history and explicit approval actions. The runtime owns database writes and can serve the separately maintained static interface. Inspect the task state, approval and safe event timeline before attempting recovery; trace data alone does not prove an external action completed. Local data and artifacts are sensitive operational data and must remain outside version control.

## Evaluation

Choose a scenario, prerequisites and mode, then compare its expected assertions with its recorded result. Offline scripted models and synthetic tools can exercise native SDK control flow without a provider. Local MCP integration adds a real protocol boundary. Neither implies a successful live provider request. Each live request needs separate explicit authorization for its exact scope; previous one-use approvals do not authorize a retry.
