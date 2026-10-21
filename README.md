# servicenow-query

An [Agent Skill](https://agentskills.io/specification) that teaches AI coding
agents to run **read-only** Table API queries against a live ServiceNow
instance with ServiceNow's official `now-sdk query` CLI
([`@servicenow/sdk`](https://www.npmjs.com/package/@servicenow/sdk)). No
custom code; auth is OAuth under your own identity.

## Prerequisites

- Node.js 20+ and `npm install -g @servicenow/sdk` (or use `npx`)
- A one-time sign-in per instance, in your own terminal:

  ```bash
  now-sdk auth --add https://<instance>.service-now.com --type oauth --alias <alias>
  ```

## Install

```bash
npx skills add AlexAlvarez092/servicenow-query
```

Or copy `SKILL.md` into your agent's skills folder (e.g.
`~/.copilot/skills/servicenow-query/`).

## Example prompts

- "What are the columns and types of the `incident` table on my dev instance?"
- "When does the Business Rule 'X' fire?"
- "List the ACLs on `sc_request`."

## Safety

Read-only (GET only). The skill instructs agents to never query production
without explicit user approval and never to reuse someone else's credentials.

## License

MIT © Alejandro Alvarez
