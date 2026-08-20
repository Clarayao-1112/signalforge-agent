# Email Reply Briefing SOP

## Trigger

When a new email arrives in the monitored program mailbox, inspect it promptly. Process only new messages that are plausibly related to Startup, VC, or program outreach.

## Exclude

Do not treat the following as valid replies:

- Out-of-office notices
- Bounces and delivery failures
- Newsletters
- System notifications
- Automated receipt confirmations
- Generic unmonitored support acknowledgements

## Match hierarchy

1. Exact sender email match
2. Sender domain and company website match
3. Email thread or message ID match
4. Company name in subject or body
5. Contact identity and signature match
6. Explicit company reference in the message

If there is exactly one high-confidence match, sync it. If there are multiple or weak matches, alert the operator and wait for confirmation.

## Reply classification

- Positive Reply
- Meeting Request
- Info Request
- Referral
- Not Interested
- Out of Office
- Bounce / Delivery Failed
- Generic Support Reply
- Needs Manual Review

## Required sync fields

For a valid, unique reply, update the lead record with:

- Outreach Stage
- Last Reply Date
- Reply Type
- Reply Summary
- Email Thread ID
- Email Link, when available
- Last Email Sender
- Last Email Sender Domain
- Last Interaction Date
- Next Action

## One-page / briefing

Immediately after a valid reply is matched, retrieve available lead data and verified public information, then send an internal briefing to the Feishu bot. Use this structure:

1. Company and contact
2. Product and business context
3. Sector, geography, and stage
4. Current outreach history and reply summary
5. Current model stack and usage, when provided
6. Main pain points
7. Program fit and commercial potential
8. Security, privacy, and compliance risks
9. Missing information and questions to ask
10. Recommended next action
11. Whether Program Manager involvement is needed

The briefing must distinguish facts, user-provided claims, and open questions. Never copy the full email body or expose sensitive content unnecessarily.

## No automatic external reply

The bot may summarize and draft a reply, but must not send an external response without explicit confirmation.

