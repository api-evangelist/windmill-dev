# Windmill (windmill-dev)

Windmill is an open-source developer platform that turns scripts (Python, TypeScript, Go, Bash, SQL, and more) into internal tools, UIs, workflows, and cron jobs. It runs as Windmill Cloud (app.windmill.dev) or self-hosted, with a distributed worker fleet executing jobs. Everything in a workspace - scripts, flows, apps, schedules, variables, resources, triggers - is addressable over a single REST API (base `https://app.windmill.dev/api` on Cloud, or `/api` self-hosted), authenticated with a Bearer token, and is the same surface the Windmill CLI and web UI use.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/apis.yml)

## Tags

- Developer Platform
- Workflows
- Internal Tools
- Job Orchestration
- Cron
- Open Source

## Timestamps

- **Created:** 2026-07-02
- **Modified:** 2026-07-02

## APIs

### Windmill Scripts API

Create, list, get, update, archive, and version scripts - the core runnables written in Python, TypeScript (Bun/Deno), Go, Bash, SQL, and other supported languages. Scripts are content-addressed by hash and pathed within a workspace.

- **Human URL:** [https://www.windmill.dev/docs/getting_started/scripts_quickstart](https://www.windmill.dev/docs/getting_started/scripts_quickstart)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Scripts
- Code
- Runnables

#### Properties

- [Documentation](https://www.windmill.dev/docs/script_editor)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Flows API

Compose scripts into directed-acyclic-graph flows with branches, loops, approvals, retries, and error handlers. Create, list, get, and update flows, and inspect their versions.

- **Human URL:** [https://www.windmill.dev/docs/flows/flow_editor](https://www.windmill.dev/docs/flows/flow_editor)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Flows
- Workflows
- Orchestration

#### Properties

- [Documentation](https://www.windmill.dev/docs/flows/flow_editor)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Apps API

Manage low-code apps - drag-and-drop UIs backed by scripts and flows. Create, list, get, and update apps, and expose public app views for sharing.

- **Human URL:** [https://www.windmill.dev/docs/apps/app_editor](https://www.windmill.dev/docs/apps/app_editor)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Apps
- UI
- Low Code

#### Properties

- [Documentation](https://www.windmill.dev/docs/apps/app_editor)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Jobs API

Trigger and manage job executions - run a script or flow by path or hash (fire-and-forget or run-and-wait-result), list queued and completed jobs, get job status and results, and cancel running jobs.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/jobs](https://www.windmill.dev/docs/core_concepts/jobs)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Jobs
- Execution
- Runs

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/jobs)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Schedules API

Schedule scripts and flows on cron expressions. Create, list, get, update, and enable/disable schedules attached to a runnable path.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/scheduling](https://www.windmill.dev/docs/core_concepts/scheduling)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Schedules
- Cron
- Automation

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/scheduling)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Variables API

Manage workspace variables and secrets - encrypted, path-scoped values injected into scripts and flows at runtime. Create, list, get, update, and delete variables.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/variables_and_secrets](https://www.windmill.dev/docs/core_concepts/variables_and_secrets)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Variables
- Secrets
- Configuration

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/variables_and_secrets)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Resources API

Manage resources and resource types - structured, typed connection objects (database credentials, API keys, cloud accounts) referenced by scripts and flows. Create, list, get, update, and delete resources and their types.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/resources_and_types](https://www.windmill.dev/docs/core_concepts/resources_and_types)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Resources
- Connections
- Integrations

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/resources_and_types)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Workspaces API

List, create, archive, and delete workspaces (isolated tenants), and read or update workspace settings, invites, and membership. Windmill resources are all scoped under a workspace.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/roles_and_permissions](https://www.windmill.dev/docs/core_concepts/roles_and_permissions)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Workspaces
- Tenancy
- Settings

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/roles_and_permissions)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Users API

Manage users globally and per workspace, log in and out, resolve the current identity (whoami), create and revoke API tokens, and manage service accounts used for automation.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/authentification](https://www.windmill.dev/docs/core_concepts/authentification)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Users
- Authentication
- Tokens

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/authentification)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Groups API

Manage user groups used for role-based access control. Create, list, get, update, and delete groups, and add or remove members.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/groups_and_folders](https://www.windmill.dev/docs/core_concepts/groups_and_folders)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Groups
- Permissions
- RBAC

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/groups_and_folders)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Folders API

Manage folders - the ownership and permission boundaries that group scripts, flows, apps, variables, and resources. Create, list, get, update, and delete folders and manage their owners.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/groups_and_folders](https://www.windmill.dev/docs/core_concepts/groups_and_folders)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Folders
- Organization
- Permissions

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/groups_and_folders)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Audit Logs API

List and retrieve audit log entries recording who did what in a workspace. Audit logs are an admin-only capability and a Windmill Enterprise Edition feature.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/audit_logs](https://www.windmill.dev/docs/core_concepts/audit_logs)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Audit
- Logging
- Compliance

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/audit_logs)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Workers API

Observe the distributed worker fleet that executes jobs - list active workers, their worker groups and tags, and read queue metrics. Compute capacity is billed in Compute Units on paid plans.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/worker_groups](https://www.windmill.dev/docs/core_concepts/worker_groups)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Workers
- Fleet
- Compute

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/worker_groups)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill Triggers API

Configure event triggers that run scripts and flows - HTTP routes, WebSocket, Kafka, NATS, Postgres, SQS, and MQTT triggers. Note that WebSocket triggers have Windmill connect OUT to an external WebSocket server as an event source; they do not expose a Windmill-hosted WebSocket API. Create, list, get, update, and delete triggers of each type.

- **Human URL:** [https://www.windmill.dev/docs/getting_started/triggers](https://www.windmill.dev/docs/getting_started/triggers)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- Triggers
- Webhooks
- Event Driven

#### Properties

- [Documentation](https://www.windmill.dev/docs/getting_started/triggers)
- [API Reference](https://www.windmill.dev/docs/core_concepts/websocket_triggers)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Windmill OIDC API

Mint short-lived OIDC (JWT) tokens from within a job so scripts and flows can authenticate to external cloud providers (AWS, GCP, Azure, Vault) without long-lived secrets. OIDC token issuance is a Windmill Enterprise Edition feature.

- **Human URL:** [https://www.windmill.dev/docs/core_concepts/oidc](https://www.windmill.dev/docs/core_concepts/oidc)
- **Base URL:** `https://app.windmill.dev/api`

#### Tags

- OIDC
- Identity
- Federation

#### Properties

- [Documentation](https://www.windmill.dev/docs/core_concepts/oidc)
- [API Reference](https://app.windmill.dev/openapi.html)
- [OpenAPI](openapi/windmill-dev-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/windmill-dev.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/windmill-dev.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/windmill-labs)
- [LinkedIn](https://www.linkedin.com/company/windmill-labs)
- [Website](https://www.windmill.dev)
- [Documentation](https://www.windmill.dev/docs)
- [Plans](plans/windmill-dev-plans-pricing.yml)
- [Rate Limits](rate-limits/windmill-dev-rate-limits.yml)
- [Fin Ops](finops/windmill-dev-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
