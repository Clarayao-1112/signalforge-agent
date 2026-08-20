# Security and Handoff

## Never publish

- App secrets
- OAuth or refresh tokens
- User IDs or chat IDs
- Mailbox addresses
- Private Feishu links
- Customer names, emails, message bodies, or lead exports
- Local paths, proxy settings, browser sessions, or CLI profiles

## New-host first run

1. Read this repository and confirm the intended business scope.
2. Ask the new owner to provide the current Feishu app, bot, mailbox, Base links, required permissions, and Program Manager contact through a secure channel.
3. Re-authenticate all external services.
4. Run read-only identity, mailbox, and Base checks.
5. Test bot delivery with a harmless message.
6. Test email-to-lead matching without writing.
7. Enable writes only after confirmation.

## Permission model

Read access should be separated from write access where possible. Batch writes, merges, status updates, and external sends require confirmation. Keep secrets in environment variables or a managed secret store.

## Event-driven operation

For timely email handling, prefer Feishu mailbox events and bot message events through a stable HTTPS callback. Polling is an acceptable fallback but should deduplicate by message and thread ID.

