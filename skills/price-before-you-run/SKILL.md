---
name: price-before-you-run
description: Before any AI or API run that costs money (a batch of API calls, an eval or benchmark, a test set, a fine-tune or training round, a long agent loop, an image or video batch), state the dollar price, which account and card pays, whether it can reach a card, and a cheaper sample run first. Use when about to spend API credits or when the user asks "how much will this cost", "is this going to hit my card" or "why did my bill jump".
license: MIT
metadata:
  author: Isla Tech LLC
  version: "1.0"
---

# Price before you run

A small business owner should never find out what an AI run cost from the card statement.
Before you start any run that spends money, say three things and wait for a yes.

## The three lines (every time)

1. **The price, at full list price.** Count times cost per call, in dollars. Example: `200 questions × about $0.03 = about $6.`
   Give the full price first, even if a credit will cover it. Then say what the credit covers.
2. **Who pays.** Which account, which credit balance, which card.
3. **Can it reach a card?** Say yes or no, and when. Auto-reload settings count: `This account reloads $20 from the card when it drops under $5.`

## Then offer the cheap way first

- **A sample run:** 10 items before 200. Example: `10 questions ≈ $0.30 first, to check the setup works.`
- **A free route** if there is one: a smaller model, a local or open-weights model, a free compute tier.
- **Batch or cache discounts** if the provider offers them.

## Plan for prices to move

- Plan as if free credits go away and token prices double. If the business case only works with free credits, say so.
- A spending cap you wrote in code is **not** a credit. Never call it "the limit used up" without saying what it is.

## While it runs and after

- Log what it spent per run, with the date and what it was for, in one place the owner can read.
- If a run will go past the price you said by more than 20%, stop and ask.
- After the run: what it cost, what it bought, and whether to run it again.

## Example

```
Before I run the full test:

Price: 200 questions × about $0.03 = about $6 at list price.
Who pays: your API account, from its $20 balance.
Card: no, unless the balance drops under $5; then it reloads $20 from your card.

Cheaper first: 10 questions for about $0.30, to check the setup.

Run the 10-question sample?
```
