---
name: plan-with-elis
description: Use only when the user explicitly asks to plan a task with Elis Token Saver, request an estimate, or report measured usage. Do not call it for routine prompts or without explicit opt-in.
---

# Plan with Elis Token Saver

This skill is an optional interface to the user's Elis account. It does not execute the underlying task; Claude remains responsible for carrying out the work using its available tools.

Use only after the user explicitly asks to plan or measure the current task. First inspect the current Token Saver tool descriptions and supported workflow. Ask Elis for an estimate; a quote alone does not reserve usage. Commit only after the user authorizes execution and any stated spend. Follow the returned task sequence and dependencies, report actual outcomes to the same plan, and finish the plan when the requested work is complete.

Do not invent token counts, savings, feedback, model switches, delegation, or completed work. If usage data is unavailable, say so. Keep the user's no-store and no-community choices. Never initiate purchases, subscriptions, or upgrades. The skill does not enable Elis community miners or send task content outside the declared Elis connector.
