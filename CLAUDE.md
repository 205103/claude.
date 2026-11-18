<!-- usage-profile:start -->
# Usage rules

## Models
- The session runs on opusplan: Opus in plan mode, Sonnet for everything else.
- Enter plan mode only when the work touches several files, changes architecture, or has unclear requirements. Skip planning for small, clear changes.
- Subagents: Explore, runner and bulk-edit run on Haiku. reviewer and general-purpose run on Sonnet. Do not pass opus or fable as a subagent model unless I ask.

## Subagents
- Work inline when one to three tool calls will finish the job.
- Delegate only when the output would be long (test runs, logs, wide searches) or the task is independent of this conversation.
- One subagent per task. Never give two subagents the same question.
- Ask each subagent for a short summary, not raw output.

## Context
- Search first, then read only the matching section with offset and limit. Do not read a whole file to find one function.
- Do not re-read a file you already read in this session unless it changed.
- Reuse earlier results and decisions instead of redoing them.
- Keep replies short. Do not restate my request or recap your steps. Explain in depth only when I ask or the change is risky.
- When I start an unrelated task, tell me to run /clear first. At a natural break in a long session, suggest /compact with a focus line.

## Compact instructions
When compacting, keep the current task and its acceptance criteria, the files changed and why, the commands that passed or failed, and open decisions. Drop exploration that led nowhere and full file contents.
<!-- usage-profile:end -->
