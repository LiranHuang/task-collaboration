# Task Collaboration

An independent agent skill for bounded delegation, role and model routing,
fallback, dependency-aware parallel work, context isolation, handoff, and agent
retirement. Use it before delegation or when receiving an agent handoff;
ordinary solo tasks skip it.

The parent owns user intent, integration, progress, and final acceptance.
Engineering execution, Git, worktrees, artifact lifecycle, and runtime adoption
follow the host project's engineering rules (optionally supplied by a skill such
as `agent-engineering-mindset`). This package has no mandatory companion skill
and does not replace runtime tools or project permissions. Role names are generic
responsibilities; model routes are configurable examples, not required providers.

## Installation

The repository root is the installable package. Place `SKILL.md` in a directory
named `task-collaboration` under the runtime's configured skill directory:

| Runtime | Typical destination |
| --- | --- |
| Codex | `~/.codex/skills/task-collaboration/` |
| DeepSeek Harness | `~/.dsh/skills/task-collaboration/` |
| OpenClaw or other compatible runtimes | Their configured `SKILL.md` discovery directory |

Refresh the catalog or start a new session as required by the host. Preserve
native task tracking and use only supported model and delegation controls.
Fallback routes require available models/providers; the skill does not implement
an automatic failover service.

## Verification

Confirm the skill appears in the runtime catalog. Independent delegation should
load it; a small solo task should remain direct. Verify actual model selection
and ownership transfer when replacing an agent.

## History and license

Extracted from `agent-engineering-mindset` with the collaboration package's Git
history preserved. MIT — see `LICENSE`.
