# 3. Log and Reflection

## Alternative questions considered, and what I checked
Variables in the data: `date`, `item`, `city`, `price`, `unit`, `data_label`. The columns were checked directly in the CSV; no separate data dictionary was supplied.

| # | Candidate question | Variables needed | Decision | Reason / evidence |
|---|---|---|---|---|
| 1 | Which item's price rose most between 1 Jan and 19 Mar? | `item`, `date`, `price` | **Accepted** | All three exist; Sweetener D +19.8% (City 1), +19.0% (City 2) |
| 2 | Is the gap between the two cities constant? | `city`, `item`, `date`, `price` | **Accepted** | City 2 − City 1 = 6.0 PKR/kg for every item and date |
| 3 | Are staples becoming unaffordable relative to wages? | wages/income | **Rejected** | No income, wage or budget variable in the file |
| 4 | Did prices rise because of the exchange rate or import costs? | exchange rate, import costs | **Rejected** | No cause variables; prices alone cannot show causes |
| 5 | Are prices rising across the whole country? | many named locations | **Rejected** | Only two anonymous cities ("City 1", "City 2"), so no national claim; also the data are illustrative |
| 6 | Do people just spend differently? | quantities / expenditure | **Rejected** | Only prices are recorded, no quantities or spending |

No source link was named for any question, so there was nothing to open and record.

## Log row
| Date | Tool / role | What I asked | What I kept | Check I ran and evidence | Accepted/Rejected |
|---|---|---|---|---|---|
| ______ | (none, per the instruction to set aside the AI-use step) | — | — | Recalculated % changes and the city gap with pandas in `2_work.ipynb`; matched by hand for Staple A City 1: 101.0 → 114.5 = +13.4% | n/a |

## Reflection (about 100 words)
My data can say how four items' weekly prices moved in two cities between 1 January and 19 March 2026. Every item ended higher, but at very different rates: Sweetener D about 19–20%, Oil B about 15%, Staple A about 13% and Pulse C under 4%. Prices also dipped in some weeks, so the start and end dates matter. The two cities move in lockstep, 6 PKR/kg apart. The data cannot say whether prices are affordable, why they moved, what people buy, or what happens nationally. There are no incomes, quantities, causes or named locations, and the file is illustrative teaching data.

## Most tempting but unsupported suggestion (3 sentences)
The most tempting question was "Are staples becoming unaffordable?" because it matches the headline wording exactly. It is unsupported because the file has prices only, with no wages, incomes or spending to compare them with. The data can show how fast Staple A's price rose (about 13%), but not whether people can afford it.
