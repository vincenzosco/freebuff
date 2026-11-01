# Freebuff

Freebuff is the public, free coding agent built from the Codebuff agent framework.

## Key Technologies

- TypeScript monorepo
- Bun runtime and package manager
- OpenTUI + React CLI
- JS/TS SDK
- Composable agent runtime

## Repo Map

- `cli/` - TUI client and local UX
- `sdk/` - JS/TS SDK used by the CLI and external users
- `common/` - shared types, tools, schemas, and utilities
- `agents/` - public agent definitions
- `packages/agent-runtime/` - agent runtime and tool handling
- `packages/code-map/` - source parsing helpers
- `packages/llm-providers/` - public LLM provider shims
- `freebuff/` - Freebuff CLI, release files, and e2e tests
- `scripts/tmux/` - tmux helpers for CLI testing

## Conventions

- Use `bun install` and `bun run`.
- Prefer dependency injection over module mocking.
- Run interactive CLI tests in tmux.
- Do not force-push `main`.

## Docs

- `docs/agents-and-tools.md`
- `docs/testing.md`



## Commits

- **Short, human, one line.** The subject says what changed, in the imperative, and
  stops at about 60 characters: `Search sixteen padding tails`, not a paragraph
  about why. Detail belongs in the code and in the pull request, not in the git log.
- **No AI attribution of any kind.** No `Generated with ...` line, no
  `Co-Authored-By: ...` trailer, no emoji footer. If a tool offers to add one, the
  answer is no.
- One commit per change that stands on its own. Dependency bumps, generated files
  and formatting are their own commits when they are not part of the change.
