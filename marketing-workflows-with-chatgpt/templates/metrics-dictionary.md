# Metrics dictionary

Define event names, source systems, time zones, identity/deduplication rules, and observation windows before combining data.

| Metric | Definition | Limit |
| --- | --- | --- |
| Link CTR | Link clicks / impressions | Impression-based, not people-based. |
| Session conversion rate | Completed target actions / eligible sessions | Match action and session scope. |
| Sample-to-order rate | Sample customers who order / eligible sample customers | Use a fixed follow-up cohort/window. |
| Cost per action | Relevant spend / completed target actions | Undefined when actions are zero. |
| Net revenue | Recorded revenue less refunds/cancellations | Confirm tax/shipping treatment. |
| ROAS | Attributed revenue / ad spend | Not profit and not causal lift. |
| Hotel qualified inquiry | Inquiry meeting agreed booking criteria | Criteria belong to the hotel owner. |
| Workflow review time | Human review minutes per comparable task | Separate from generation/wait time. |

Keep unknown cells blank, not zero. Do not merge sample requests, sample purchases, final wallpaper orders, and hotel bookings into one conversion total. Do not add platform-reported conversions without deduplication.
