---
created: 
basis: TBD
tags:
---

# Claude Code Quick Reference — Commands, Shortcuts & Tips

---

## Slash Commands

| Command                                         | Purpose                                 | Pro Tip                                                                   |
| ----------------------------------------------- | --------------------------------------- | ------------------------------------------------------------------------- |
| /Advisor                                        | Get a better model second opinion       |                                                                           |
| /caveman                                        |                                         |                                                                           |
| `/clear`                                        | Wipe conversation history, free context | Use when starting a new unrelated task. Delete old content to save tokens |
| /context                                        | breaks down your current content        |                                                                           |
| `/effort low`, `/effort medium`, `/effort high` | Adjust effort level                     | Use to change the degree of effort for more desired results               |
| `/compact [instructions]`                       | Summarize conversation to save context  | Add focus: `/compact focus on code changes`                               |
| `/memory`                                       | View/edit your CLAUDE.md auto-memory    | Review/correct what Claude remembers about you                            |
| `/config`                                       | Open settings GUI                       | Change model, permissions, themes                                         |
| `/model`                                        | Switch AI model on the fly              | `sonnet` (balanced), `opus` (hard problems), `haiku` (fast/cheap)         |
| `/btw <question>`                               | Ask a quick side question               | Does NOT add to conversation history                                      |
| `/cost`                                         | See token usage stats                   | Gauge when to `/compact`                                                  |
| `/context`                                      | Visualize context window usage          | Color grid showing what's consuming tokens                                |
| `/plan`                                         | Enter read-only analysis mode           | Claude thinks without executing anything                                  |
| `/diff`                                         | View uncommitted file changes           | Useful before committing                                                  |
| `/init`                                         | Create a `CLAUDE.md` for a project      | Sets persistent project-specific instructions                             |
| /insites                                        | Suggest ways to work 10x faster         |                                                                           |
| `/fork`                                         | Branch the conversation                 | Explore an alternative without losing main thread                         |
| /remote-control                                 | control Claude Code from your phone     |                                                                           |
| /rename                                         | Gives your current chat a new name      |                                                                           |
| /resume                                         | pick up where you left off              |                                                                           |
| `/rewind`                                       | Roll back conversation + code changes   | Undo last action                                                          |
| `/skills`                                       | List available skills                   | See all `/skill-name` commands available                                  |
| /skill-creator                                  | Create skills with benchmarks           |                                                                           |
| /statusline                                     | show cost and progress bars             |                                                                           |
| `/help`                                         | Show all commands                       | Built-in reference                                                        |
| /ULTRATHINK                                     | Smartest thinking mode                  |                                                                           |
| `/voice`                                        | Speak commands                          |                                                                           |

---

## Keyboard Shortcuts

| Shortcut | Action |
|---|---|
| `Ctrl+C` | Cancel current generation mid-stream |
| `Ctrl+L` | Clear terminal screen (keeps history) |
| `Esc` + `Esc` | Rewind conversation to previous point |
| `Shift+Tab` | Cycle permission modes (auto/ask/manual) |
| `Ctrl+T` | Toggle task list visibility |
| `Ctrl+O` | Toggle verbose output (see full tool details) |
| `Alt+P` | Switch model without clearing your prompt |
| `\ + Enter` | Multiline input (works in any terminal) |
| `Ctrl+F` | Kill all background agents (press twice) |
| `Ctrl+G` | Open prompt in external text editor |

---

## High-Value Tips

- **`/compact` early** — Compact before context fills up, not after. Add focus instructions to keep what matters.
- **`/plan` before edits** — Use plan mode to review Claude's approach before it touches important files.
- **`/fork` for iteration** — Branch off to try a different angle without losing your main conversation thread.
- **`/btw` for quick questions** — Ask side questions mid-task without derailing context or history.
- **`Ctrl+C` to interrupt** — If Claude goes in the wrong direction, cancel immediately and redirect rather than waiting.
- **`Esc+Esc` to rewind** — Rolls back both the conversation AND any code changes made in the last turn.
- **`Shift+Tab` to control permissions** — Cycle between auto-approve, ask-each-time, and manual modes on the fly.
- **`/memory` check periodically** — Review stored preferences to keep Claude's behavior accurate over time.

**When instructing to save content.** 
"Save this verbatim — deduplicate with note improvements."

  When you say that, I will:
  1. Read the relevant existing file(s) first
  2. Identify what's already there vs. what's new
  3. Merge the new content in without repeating what exists
  4. Flag any suggested improvements as a short note at the bottom — not embedded in the content, so you can accept or ignore them separately
  5. Confirm the save with the file path

  If the right destination file is ambiguous, I'll ask before touching anything.
