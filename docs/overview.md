# Overview

OAS has two related purposes: provide durable, bounded execution of registered tasks and investigate the native Python Agents SDK using reproducible scenarios. The umbrella owns cross-component contracts, shared scripts, evidence, and the component manifest. Four independent repositories own the runtime, console, synthetic MCP fixture, and controlled sample service. Their code is not shared through imports of private source trees.

The original specification is a requirements baseline, not evidence of implementation. The local inspection found newer changes beyond published checkpoints. This handbook describes those observations as local unless a specific published source is established. The umbrella remote could not be independently verified and is therefore not linked.

The system is intentionally smaller than a general workflow product: the runtime manages tasks, state and SDK interactions; the console is an API client; external queues and distributed scheduling are future integration concerns. The local service is not a substitute for production authentication, transport security, multi-user authorization, or a complete data retention policy.
