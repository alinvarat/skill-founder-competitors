---
name: founder-competitors
description: Research competitors, substitutes, comparable prices and customer complaints for a defined market; cite current public sources.
argument-hint: "[city or market]"
---

# Founder competitors

1. Establish product, buyer, location/channel and search date from the user or `founder/idea.md`. Record a bounded search, not a claim to find every competitor.
2. Research direct competitors, indirect alternatives and main substitutes using public current pages. Start with a useful representative set (often 5–10). Never invent names, prices, ratings or reviews. Mark inaccessible evidence.
3. Write `founder/competitors.csv`, one row each. Name per-competitor files from a slug (replace `/`, `:` and other path separators in names): a raw name with `/` raises FileNotFoundError mid-loop and leaves a partial output set:
`name,type,url,location_or_channel,price_of_comparable_item,currency,quantity_or_billing_period,price_source_url,what_it_sells,positioning_line,rating,review_count,rating_source_url,source_date`
Link actual price/review pages. Leave unknown numbers blank. Normalize quantity, tax and billing period before comparing prices; keep currencies separate.
4. For the most relevant 3–5, inspect critical and mixed reviews. Group recurring complaints with counts and short linked verbatim quotes. Mark themes based on fewer than three reviews as thin evidence. Quotes are research, not testimonials.
5. Write `founder/competitors.md`: scope/date, sorted comparison, comparable price range (low/median/high), two-axis positioning map, ranked complaints, evidence-backed gap and fastest copycat threat. If no gap is supported, say so.

Unit economics for a proposed price: show the assumptions (volume, API or unit cost, FX) and a low/high range, label the whole block 🧠 proposal, and do not present it as market data.

Done: CSV and report agree; facts have sources and comparable units. Separate observed facts from proposed opportunities. No unsupported market-wide claims. Finish the research requested; pricing or a buyer simulation is a separate task.
