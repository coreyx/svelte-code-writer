# Svelte Code Writer Skill

A Kiro skill that provides CLI tools for Svelte 5 documentation lookup and code analysis.

## What This Skill Does

This skill enables Kiro to work more effectively with Svelte 5 projects by providing:

- Documentation lookup for Svelte 5 and SvelteKit
- Code analysis and autofix suggestions for Svelte components
- Rune-aware syntax checking ($state, $derived, $effect, etc.)

## Installation

### Import into Kiro IDE

1. Open the Agent Steering & Skills section in the Kiro panel
2. Click the + button and select "Import a skill"
3. Choose your import source:
   - GitHub: Paste the URL to the folder containing SKILL.md or directly to the SKILL.md file
   - Local folder: Browse to where you've cloned this repository and select the folder containing the skill

Once imported, the skill is automatically copied to your skills directory and ready to use.

### Manual Installation

You can also manually place the skill file at:
- User-level: `~/.kiro/skills/svelte-code-writer/SKILL.md`
- Workspace-level: `.kiro/skills/svelte-code-writer/SKILL.md`

For the latest installation instructions, see the [official documentation](https://kiro.dev/docs/skills/).

## Activation

Once installed, the skill will be automatically available to Kiro. You can activate it manually in chat using:

```
#svelte-code-writer
```

Or Kiro will automatically use it when working with Svelte files.

## Requirements

- Node.js and npm/npx installed
- The `@sveltejs/mcp` package (automatically fetched via npx)

## Alternative: Svelte MCP Power

For a more integrated experience, consider installing the Svelte MCP Power instead, which provides the same functionality through Kiro's Power system.

See https://github.com/coreyx/svelte-mcp-power

## Usage

The skill provides three main commands:

- `npx @sveltejs/mcp list-sections` - List available documentation
- `npx @sveltejs/mcp get-documentation "<sections>"` - Get specific docs
- `npx @sveltejs/mcp svelte-autofixer "<code_or_path>"` - Analyze and fix code

See SKILL/SKILL.md for detailed usage examples.
