# Blackjack Hand Evaluator

Python practice project that models the core rules of Blackjack (21): card values, soft Aces and hand totals.

Forked from [ThatoMapheto/black_jack](https://github.com/ThatoMapheto/black_jack) and worked on during the WeThinkCode_ bootcamp.

## What it does

- Maps each card rank to its value (2 to 10 at face value, J/Q/K = 10, A = 11).
- Calculates a hand's total, automatically counting Aces as 1 instead of 11 when the hand would otherwise go over 21.
- Parses a decision point written as `hand | dealer card | first/later`, for example `10,6 | 9 | first`.

## Files

| File | Purpose |
|-|-|
| `new.py` | Card values, hand total and decision-point parsing |
| `black_jack.ipynb` | Notebook used to explore and test the logic step by step |

## Running it

Requires Python 3.

```bash
python new.py
```

Or open `black_jack.ipynb` in Jupyter or VS Code and run the cells.

## Example

```python
hand_values(["A", "K"])        # 21
hand_values(["A", "9", "5"])   # 15  (Ace counted as 1)
```
