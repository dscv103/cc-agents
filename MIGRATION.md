# Claude Code Migration

This migration replaces all SDLC orchestration and GitHub Copilot agent configurations with Claude Code sub-agents and skills, improving modularity and context control.

## Sub-Agents Location
- All project-level sub-agents are now found in `.claude/agents/`
- YAML frontmatter is used per Claude agent spec
- See sub-agent file for role, workflow, handoff, and tips

## Changes made
- Fully migrated 12 Copilot agents to `.claude/agents/` in Claude format
- Updated all agent descriptions, tool lists, and invocation logic for compatibility with Claude's orchestration
- Preserved SDLC handoff and ownership details per existing workflow
- Updated role files for requirements, design, implementation, testing, QA, bug fixes, DevOps, release, documentation

## Next steps
- Test workflows using Claude CLI or in-editor Claude integration
- Refactor documentation: README.md and PROJECTSTATE.md to reflect new agent structure
- Archive `.github/agents/*` (can be removed after validation)
- Train team on using `/agents` and `/skills` commands in Claude Code interface

## Reference
- See Claude agent/sub-agent docs for advanced configuration