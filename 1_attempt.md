# 1. Attempt (THINK stage)

## Two vague claims about prices
1. "Everything costs more."
2. "Staples are out of reach."

## One answerable question per claim
| Claim | Answerable question | Variable needed |
|---|---|---|
| 1. Everything costs more | Between 1 Jan and 19 Mar 2026, by what % did each item's price change in each city, and did it rise every week? | `price` by `item`, `city`, `date` |
| 2. Staples are out of reach | Did Staple A's price rise faster or slower than the other items, and does that differ between cities? | `price` for Staple A vs other items, by `city` |

Why these are testable: each names an item, a place, a period, a unit (PKR per kg) and a comparison.
What they leave out: "out of reach" is about affordability, which needs incomes or budgets that the price file does not contain.

## Predictions before running code
> **Fill these in with your own genuine guesses made BEFORE you ran any code. Criterion B is marked on this.**
> Note: I (Claude) looked at this file before writing these notes, so I cannot honestly supply a "before" prediction for you.

- Predicted shape (rows, columns): ______
- Predicted number of distinct items: ______
- Predicted number of distinct dates: ______

(Actual values are in `2_work.ipynb`: shape (96, 6), 4 items, 12 dates.)

## Snapshot
- Commit message: `attempt-before-AI`
- Commit hash: ______ (paste the output of `git log -1 --format=%H`; it must be dated before your first AI log entry)
