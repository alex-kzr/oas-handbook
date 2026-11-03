# Development and operations

Python tooling targets WSL2. The runtime requires Python 3.12 and uses uv with locked official dependencies. Each component owns its own tests and dependency manifest. Obtain the independently maintained checkouts through their verified repository links and verify the desired commits and access permissions. The umbrella uses submodules; initialize and check them only after obtaining a verified umbrella source. A remote branch may not include the local checkpoint described here.

From an inspected runtime checkout with its locked dependencies already available, the documented offline unit-test pattern is:

```text
uv run --offline --locked python -m unittest discover -s tests/offline -v
```

Dependency synchronization can require network access; do it only under the applicable local policy. Offline tests use synthetic fixtures and do not validate paid providers. MCP integration, browser checks and Docker experiments have separate prerequisites and are not implied by an offline unit-test pass. Review the component's own instructions for its current revision before running anything.

Keep runtime state in the configured ignored `.agents-data` root, or an explicitly configured private data root. Do not commit logs, checkpoints, credentials, generated artifacts, disposable workspaces or user data. The console communicates through the runtime API and must not bypass its approval controls. Protect backups and review retention separately; a synthetic cleanup fixture is not a comprehensive retention policy.

For diagnosis, check the selected mode, component availability, configuration presence, task state, recorded safe errors and approval status. Missing prerequisites should block the affected operation rather than silently switch modes. An interrupted or uncertain action may need a new reviewed request; avoid automatic replay. Live models, transmission of user data, credentials and Docker resource use require the applicable separate authorization. Local single-operator safeguards do not establish production security.
