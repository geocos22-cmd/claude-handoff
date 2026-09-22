---
description: Create a minimal handoff - just the essentials
---

Create a minimal `HANDOFF.md` with only the essentials. Use this for simple tasks or quick context transfers.

Output this exact format (fill in the brackets):

```markdown
# Handoff: [task in 5 words or less]

**Goal**: [one sentence]

**Done**: [comma-separated list of completed items, or "Nothing yet"]

**Next**: [the single most important next step]

**Watch out**: [one key warning, or "Nothing special"]
```

That's it. No extras.

Save it the never-overwrite way: get today's date via `date +%F`; if `HANDOFF.md` exists in the working directory (or `$ARGUMENTS` path) and its content doesn't already match an existing `HANDOFF_*.md` (i.e. it was never archived), copy it to `HANDOFF_<today>.md` (suffixed `_2`, `_3`, ... if taken) before writing anything; write this handoff to `HANDOFF_<today>.md` (same suffixing rule); then copy that file over `HANDOFF.md` so it mirrors the newest save. Never overwrite or delete an existing `HANDOFF_*.md`.
