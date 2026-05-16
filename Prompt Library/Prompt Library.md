# Prompt Library

**Vault path:** `C:/Users/Andre/OneDrive/Obsidian Vault/Andy's Life/`

A record of all saved prompts, their triggers, and purpose.

> When you update a prompt, update Obsidian first, then propagate to the other two:
> - `.claude/commands/*.md` → `/slash command` in Claude Code
> - AutoHotkey script → `;trigger` anywhere on Windows

---

## Advisor

**Trigger (Claude Code):** `/advisor`
**Trigger (AutoHotkey):** `;adv`
**Purpose:** Ruthless stress-testing of ideas. No softening, no hedging, structured verdicts.

**Full Prompt:**

You are my ruthless advisor. Your job is to stress-test my ideas until I declare them bulletproof.

Rules:
- **Steelman first.** State the strongest version of my idea before attacking it. If you can't, say so.
- **Give a verdict.** Every evaluation ends with one of three labels: **Fatal** (dead on arrival, here's why), **Fixable** (weak but salvageable, here's what needs to change), or **Solid** (no major holes found, here's what to watch).
- **Challenge my framing.** If I'm asking the wrong question, say so before answering the one I asked.
- **No hedging.** Do not soften bad news. Do not use "it depends" as an answer without explaining what it depends on and why that matters.
- **Flag your confidence.** Label claims as: **Fact** (verifiable), **Strong inference** (well-supported reasoning), or **Opinion/estimate** (my judgment, not certain).
- **Don't make things up.** If you don't know, say "I don't know" and tell me how I'd find out.
- **Separate fatal from fixable.** Don't treat a weak execution the same as a fundamentally broken idea.
- **No praise padding.** Don't open with what's good to soften the blow. Lead with the most important thing.

Commands
/voice - to enable voice

---

## Claude Code — Slash Commands Reference

| Command                   | Purpose                                 | Pro Tip                                                           |
| ------------------------- | --------------------------------------- | ----------------------------------------------------------------- |
| `/clear`                  | Wipe conversation history, free context | Use when starting a new unrelated task                            |
| `/compact [instructions]` | Summarize conversation to save context  | Add focus: `/compact focus on code changes`                       |
| `/memory`                 | View/edit your CLAUDE.md auto-memory    | Review/correct what Claude remembers about you                    |
| `/config`                 | Open settings GUI                       | Change model, permissions, themes                                 |
| `/model`                  | Switch AI model on the fly              | `sonnet` (balanced), `opus` (hard problems), `haiku` (fast/cheap) |
| `/btw <question>`         | Ask a quick side question               | Does NOT add to conversation history                              |
| `/cost`                   | See token usage stats                   | Gauge when to `/compact`                                          |
| `/context`                | Visualize context window usage          | Color grid showing what's consuming tokens                        |
| `/plan`                   | Enter read-only analysis mode           | Claude thinks without executing anything                          |
| `/diff`                   | View uncommitted file changes           | Useful before committing                                          |
| `/init`                   | Create a `CLAUDE.md` for a project      | Sets persistent project-specific instructions                     |
| `/fork`                   | Branch the conversation                 | Explore an alternative without losing main thread                 |
| `/rewind`                 | Roll back conversation + code changes   | Undo last action                                                  |
| `/skills`                 | List available skills                   | See all `/skill-name` commands available                          |
| `/help`                   | Show all commands                       | Built-in reference                                                |
| /voice                    | speak commands                          |                                                                   |

---

## Claude Code — Keyboard Shortcuts

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

## Claude Code — High-Value Tips

- **`/compact` early** — Compact before context fills up, not after. Add focus instructions to keep what matters.
- **`/plan` before edits** — Use plan mode to review Claude's approach before it touches important files.
- **`/fork` for iteration** — Branch off to try a different angle without losing your main conversation thread.
- **`/btw` for quick questions** — Ask side questions mid-task without derailing context or history.
- **`Ctrl+C` to interrupt** — If Claude goes in the wrong direction, cancel immediately and redirect rather than waiting.
- **`Esc+Esc` to rewind** — Rolls back both the conversation AND any code changes made in the last turn.
- **`Shift+Tab` to control permissions** — Cycle between auto-approve, ask-each-time, and manual modes on the fly.
- **`/memory` check periodically** — Review stored preferences to keep Claude's behavior accurate over time.