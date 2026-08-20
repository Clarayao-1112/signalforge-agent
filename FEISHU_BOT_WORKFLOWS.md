# Feishu Bot Workflows

## Bot role

The Feishu bot is the daily interface for Program Leads Operations. It should read real tables, answer operational questions, propose changes, request confirmation, and deliver proactive alerts.

## Natural-language commands

- Today's outreach
- Second-touch list
- New replies
- High-priority leads
- View company: `<company>`
- Prepare follow-up: `<company>`
- Prepare meeting briefing: `<company>`
- Sync sales conversions
- Find duplicates
- Enrich contacts
- Weekly report

## Bot response types

### Read-only response

Return records, counts, status, evidence, and next action. No write required.

### Proposed change

Show the record, field, old value, new value, source, confidence, and reason. Add Confirm / Cancel controls.

### Batch action

Show scope, number of records, exclusions, duplicate count, and exact action. Require explicit confirmation.

### Proactive notification

Send daily outreach reminders, new valid-reply alerts, meeting requests, bounce alerts, conversion mismatches, and missing-data alerts.

## Daily reminder

At the configured local business time, send:

1. First-touch leads, prioritized.
2. Second-touch leads whose first outreach is at least seven days old, without an effective reply, and with an available channel.
3. Records missing Website, Contact, LinkedIn, X, or Last Outreach Date.

Do not send outreach from the reminder.

## Interaction safety

The bot may automatically fill empty fields only for unique, high-confidence matches under an explicitly approved rule. It must request confirmation for ambiguous matches, bulk edits, sends, merges, and destructive actions.

## Required Feishu capabilities

- Bot private-message send
- Private-message receive event for interactive commands
- Interactive card responses
- Feishu Base read/write
- Mailbox read access
- Optional calendar and document access
- Stable HTTPS event callback for event-driven operation

Polling can be used as a fallback, but event callbacks are preferred for timely mail-reply handling.

