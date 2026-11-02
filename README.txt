THE INVOICE CHASER — free giveaway from the Build It With AI channel (Episode 19)

USE THIS ONE:
  index.html          — THE FINISHED TOOL. Open it in any browser (works offline).
                        Click "Load the fictional sample books" to try it, or paste
                        your own invoices.csv / payments.csv exports. Set the books'
                        as-of date, press "Run the chaser".

SAMPLE BOOKS (entirely fictional — every address is @example.com):
  invoices.csv        — 28 rows for Bentwood Joinery
  payments.csv        — 12 payments

THE SECOND OPINION:
  checker.py          — the independent Python implementation of the same written
                        rules. Run: python3 checker.py invoices.csv payments.csv
                        '{"asOf":"2026-11-02"}'. In our tests the page and this
                        checker agreed on 40,569 values across 210 paired runs.

THE PROMPTS:
  PROMPTS.txt         — all three prompts from the episode, word for word.

THE WRECKAGE (kept so you can see what the episode caught — do NOT use these):
  engine_v1.js        — FIRST DRAFT, NOT THE TOOL. Matches payments by client name,
                        trusts the status column, drops quoted-comma rows silently.
  engine_v2.js        — SECOND DRAFT, NOT THE TOOL. Loses day-30 invoices between
                        buckets, chases overpayments, reads the machine clock.

WHAT IT WILL NOT DO: it sends nothing and charges nobody. It drafts the emails and
opens them in YOUR mail app; the send button stays yours.
