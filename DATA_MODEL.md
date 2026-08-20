# Data Model

## Core lead fields

- Lead Type
- Company Name
- Funding and stage
- Country or region
- Field or focus
- Owner
- Contact
- Website
- Notes
- Outreach Stage
- Outreach Method
- Last Outreach Date
- Last Reply Date
- Reply Type
- Reply Summary
- Next Action
- Priority
- Source metadata
- Dedup Key
- Email Thread ID
- Conversion Source
- Conversion Time
- Linked Sales Record ID

## Status values

- 待触达
- 第一次触达
- 第二次触达
- 未回复
- 已回复
- 已建联
- 已转交
- 已转化
- 已拒绝
- 暂缓
- 需补联系方式
- 需人工确认

## Enrichment rules

Prefer official websites, company domains, verified company social accounts, and public sources. Do not guess email formats. Personal email addresses may be retained as candidates but should be clearly marked and are not automatically the best business channel.

## Conversion sync

When the sales pipeline owner matches the approved conversion owner and the company match is unique and high-confidence, update the corresponding lead as converted and record source, time, and linked sales record. Do not update ambiguous matches automatically.

