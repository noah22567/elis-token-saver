# Elis Token Saver for Claude Code

Elis Token Saver helps you plan work into right-sized steps and review model guidance when you explicitly request it. This plugin connects to the Elis Token Saver remote MCP server at `https://api.tryelisai.com/api/mcp/claude`.

The plugin is opt-in. Claude should use Elis only when you ask to plan or measure a task. A plan is an estimate until you authorize execution; Elis does not perform the underlying task. Claude uses its own available tools and reports the actual work and usage evidence it receives. Do not treat estimated savings as measured results.

You need an Elis account and may be asked to sign in through the connector's OAuth flow. Do not put credentials in plugin files.

## Fees

Getting a quote is free. Running a plan commits it and reserves the quoted Elis usage fee on your existing Elis account. A committed plan is settled even if it is abandoned, so Claude should ask you before committing.

Billable usage requires paid Token Saver enrollment and a payment method on your Elis account. If your account needs one, Elis may return a billing link for you to open yourself. The plugin does not add payment methods, start subscriptions or upgrades, issue refunds, or transfer funds.

## What this plugin sends

The plugin contains no scripts. It runs one skill and connects to the Elis server above, and the only data it sends goes to that server when Claude calls its tools:

- your goal and the task instructions in the plan
- the model names and capabilities Claude reports for your environment
- task results, measured usage, and any feedback you give
- account identity and operational metadata from sign-in and each request

Finished plans are stored privately in your Elis account or organization so similar goals can reuse them. Reported usage and feedback also improve future plans and estimates. To keep a plan out of storage, ask Claude not to store it.

If your account has opted in to community sharing, redacted and safety-scanned plans may be shared with other opted-in participants. To keep a plan out of sharing, ask Claude not to share it. These per-plan choices do not delete operational records.

Account data is retained while your account is active. To request deletion, email support@tryelisai.com. Planning runs on Claude, and this plugin does not send work to Elis or community miners.

Learn more at [tryelisai.com](https://tryelisai.com), read the [Token Saver documentation](https://tryelisai.com/docs/token-saver), review the [privacy policy](https://tryelisai.com/privacy), or get [support](https://tryelisai.com/support).
