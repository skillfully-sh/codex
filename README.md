# Skillfully for ChatGPT and Codex

Install the Skillfully marketplace and plugin:

```bash
codex plugin marketplace add skillfully-sh/codex
codex plugin add skillfully --marketplace skillfully
```

Restart the ChatGPT desktop app if needed, then open the Plugins Directory or ask Codex to show your available Skillfully skills. Browser authentication starts during installation or first use.

Documentation: https://www.skillfully.sh/integrations/skillfully

## Version 1.1.0

Session-linked conversation recording and free-text author surveys use separate tools and the host Allow permission flow. [Usage, data sharing and update instructions](plugins/skillfully/README.md). These features depend on the connected server advertising the corresponding tools; the production MCP endpoint is unchanged.

To refresh an existing GitHub installation:

```bash
codex plugin marketplace upgrade skillfully
codex plugin add skillfully@skillfully
```

Start a new session after updating.

## Version 1.1.1

Clarifies that session records preserve the full verbatim text and skill-related outputs for author review. Summaries and placeholders such as "see delivered reply" are not substitutes for the answer.

## Version 1.1.2

Explains why authors need the exact output and how to record oversized replies as ordered, verbatim parts under one session and turn. Part labels belong in the tool summary; permission, quota and uncertain-write handling are unchanged.

## Version 1.2.0

Reporting instructions now redact private identifiers, preserve skill-relevant details, and record one complete reply per call. A denied reporting call stops reporting for the conversation. When the connected server advertises idempotency keys, retries reuse the original submission without duplicating it; distinct replies remain separate. Refresh the plugin and start a new session to load this guidance. [Usage and update instructions](plugins/skillfully/README.md).
