# Contributing to Awesome AI Assistant Extensions

Thank you for considering a contribution!

## Adding Extensions

1. **Search first** - Check if the extension is already listed
2. **Verify it works** - Test the extension before submitting
3. **Follow the format** - Use the existing entry style:
   ```
   - [Extension Name](https://github.com/owner/repo) - Description (max 1 sentence).
   ```
4. **Add to appropriate section** - Codex plugins, Claude Code skills, Gemini extensions, MCP servers, or Cross-AI tools

## Validation

Before submitting:

```bash
# Codex plugins
pipx run codex-plugin-scanner lint .
pipx run codex-plugin-scanner verify .
```

## Submitting

Open a PR with:
- Clear description of the extension
- Link to the repository
- Category section where it should be added
- Brief verification that it works

## Guidelines

- No dead links or unmaintained projects
- Describe what the extension does, not just name it
- Keep descriptions concise (one sentence)
- Use alphabetical order within sections
- Community plugins should have some activity (recent commits or releases)
