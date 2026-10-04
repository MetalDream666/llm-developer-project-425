### Hexlet tests and linter status:
[![Actions Status](https://github.com/MetalDream666/llm-developer-project-425/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/MetalDream666/llm-developer-project-425/actions)

Help Desk agent based on Yandex AI Studio. A project of the LLM engineer profession from the “LLM Developer” course at the Hexlet online school.

This is an e-mail support agent for company employees. The agent receives inquiries via e-mail, searches for a response in the corporate knowledge base (documentation, FAQ, regulations), and, if no ready‑made answer is found, creates a ticket and saves the correspondence in the database. The entire solution operates within the Yandex Cloud ecosystem -- without external trackers like Yandex Tracker.

### Pre-requisites

The following conditions must be met to work with the agent.

#### Service account

A service account `ai-studio-sa` has been created to work with the agent.

#### Roles

The above service account was assigned the following roles:

- `functions.functionInvoker` -- for calling Yandex Cloud Functions;
- `serverless.mcpGateways.invoker` -- for working with MCP gateways;
- `lockbox.payloadViewer` -- for reading secrets from Lockbox;
- `ai.languageModels.user` -- for querying Yandex AI Studio models;
- `ydb.editor` -- for managing the structure and data of the YDB databases.

#### Secrets

The following secrets are needed to work with the agent:

- `ydb-endpoint` -- gRPC endpoint for connecting to the YDB database;
- `ydb-database` -- the full path to the YDB database in the Yandex Cloud.


