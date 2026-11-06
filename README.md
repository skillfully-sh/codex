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
