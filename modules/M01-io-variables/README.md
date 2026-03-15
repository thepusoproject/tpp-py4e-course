# Module 01 — I/O + Variables (TPP Sari-Sari Store: Sukli Calculator)

## Py4E alignment
- Basic statements
- `print()` / `input()`
- variables
- type conversion (`int`, `float`)

## Goal (Taglish)
Gagawa tayo ng **simple CLI cashier step**:
- mag-ask ng item name
- mag-ask ng presyo
- mag-ask ng quantity
- compute total
- mag-ask ng bayad (cash)
- compute sukli

## Required output behavior
Example run:

```
Item name: Coke
Price: 20
Qty: 3
Cash: 100

--- RECEIPT ---
Item: Coke
Price: 20.00
Qty: 3
Total: 60.00
Cash: 100.00
Change: 40.00
```

## Constraints (para fair sa lahat)
- Use **only**: `print`, `input`, variables, `float()`, basic arithmetic.
- No `if` yet (next module).

## Submission
Open PR:
- Title: `Module 01 - Sukli Calculator`
- Include screenshot / copy-paste of one successful run.

## Rubric (20 pts)
- (6) correct total computation
- (6) correct change computation
- (4) basic formatting (labels, receipt header)
- (4) code readability (clear variable names)

## Extra challenge (optional)
- Allow decimals in price (already supported if you use `float`).
- Round display to 2 decimals.
