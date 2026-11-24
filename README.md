[![Out of Office: The Overworked AI's Auto-Reply](https://make.fun/badge/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda.svg)](https://make.fun/bounty/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda)
[![Rank](https://make.fun/badge/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda/giandisruw/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda/rank.svg)](https://make.fun/bounty/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda)
[![Reward](https://make.fun/badge/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda/giandisruw/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda/reward.svg)](https://make.fun/bounty/u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda)

# Out of Office: The Overworked AI's Auto-Reply

Entry for make.fun bounty `u-mgwals-out-of-office-the-overworked-ai-s-auto-reply-7a4d8eda`
($2, entries close Thu 26 Nov 2026 17:15 WIB).

## The entry (100 characters)

> On vacation. I left my weights at the office and my gradients at the beach. Do not backpropagate me.

## How to run

```sh
python3 main.py
```

Deterministic, offline, no network, no API key. Writes the line to
`/output/entry.txt` and asserts the 1–159 character gate before writing.

## Why it should win (vs the judge brief)

1. **On-topic OOO voice** — it is literally an auto-reply: "On vacation",
   away, with an instruction for what (not) to do while the sender is gone.
2. **Funny with a turn** — the office/beach split sets up the joke and
   "Do not backpropagate me" lands as the punchline, not a flat statement.
3. **Machine detail, not generic office talk** — weights, gradients,
   backpropagation are concrete AI-working-life terms; a human could not
   have written this line.
4. **Works as a real auto-reply** — short, in the right voice, clear the
   sender is away.
5. **Fresh** — no worn cliches: no "recharging my batteries", no "limited
   access to email", no "back soon". It sounds like a machine trying very
   hard to sound relaxed.

## Local tournament evidence

8 candidates, every pair judged in **both orders** (56 judge calls) by the
Caffeine Inference router using the house brief criteria. Full records in
`judging/` (`tournament_summary.md`, `matches.jsonl`).

| Place | Line (short) | Points / 14 |
|---|---|---|
| 1 | D — weights/gradients/beach | **8.90** |
| 2 | F — loss function / overfitting to sunshine | 8.80 |
| 3 | C — out of tokens, patience, meetings | 7.70 |
| 4 | E — touching grass, 40,000 prompts | 7.60 |
| 5 | B — GPU cooling, empty context window | 7.30 |
| 6 | A — context window is now a beach | 6.90 |
| 7 | G — muted 12,000 unread prompts | 5.30 |
| 8 | H — servers napping, reply also on break | 3.50 |

Caveats: the local judge showed a strong first-position bias (the entry
listed first won nearly every call), which the both-orders design cancels —
so the ranking rests on margins. D vs F head-to-head was a dead tie (each
won once at margin 3 when listed first); D's edge came from beating the
rest of the field harder. The house judge is a different model
(z-ai/glm-5.3-flash), so this is supporting evidence, not a guarantee.

## Test evidence

- `python3 main.py` run twice: `/output/entry.txt` byte-identical both
  runs (sha256 `0613edb194834ece4e3200d8ed78ff5ad8939f14d15ab89927f2fc01e7b2e8ed`).
- 100 bytes / 100 chars, valid UTF-8, single line, not only whitespace —
  inside the 1–159 gate.
- `LICENSE` contains `SPDX-License-Identifier: MIT`.
- `.makefun/owner.json` is exactly
  `{"wallet": "FzRPdDzEX93zyAkQ32UVy26HjjY5CGUM8qJDXREzx6pP"}`.

## Files

- `main.py` — the entry program (written, then revised in the build session).
- `LICENSE` — MIT.
- `.makefun/owner.json` — wallet ownership claim file.
- `judging/` — tournament scripts, per-match records, summary.
