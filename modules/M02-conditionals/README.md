# Module 02 — Conditionals (TPP Store: Discount + Stock Guard)

## 0) Py4E alignment
- Chapter 3: Conditional execution
- Concepts: `if/elif/else`, boolean expressions, comparisons, `try/except` (light)

## 1) Learning outcomes (Taglish)
After this module, kaya mo na:
- gumawa ng rules gamit `if/elif/else`
- mag-validate ng input (basic)
- mag-handle ng common errors (optional `try/except`)

## 2) Lesson (short)
**Big idea:** Programs make decisions based on conditions.

Common mistakes:
- `=` vs `==`
- comparing strings vs numbers (need `int()`/`float()`)

## 3) Micro-drills
1) Pass/Fail checker:
   - input score (0–100)
   - print "PASS" if >= 75 else "FAIL"
2) Min of two numbers
3) Safe number input (optional): use `try/except` so it doesn’t crash on non-number

## 4) Lab — Feature: Discount + Stock Guard
### User story
As a sari-sari store cashier, I want the system to apply discount rules and stop selling items kapag out-of-stock.

### Requirements
- Ask:
  - item name
  - price
  - qty
  - stock available
  - cash
- If `qty > stock`, print an error and **do not** compute receipt.
- Discount rule:
  - if `qty >= 10` → 5% discount
  - else no discount
- Print receipt showing:
  - subtotal
  - discount amount
  - total after discount
  - change

### Constraints
- Use only: `input`, `print`, variables, arithmetic, `if/elif/else`, (optional) `try/except`.
- Still no loops yet.

### Example run
```
Item name: Candy
Price: 2
Qty: 12
Stock: 20
Cash: 50

--- RECEIPT ---
Subtotal: 24.00
Discount: 1.20
Total: 22.80
Change: 27.20
```

## 5) Mastery Gate (80%)
### A) Reflection (PR description)
1) Explain (Taglish) difference ng `=` at `==`.
2) Paano mo chine-check yung out-of-stock condition?
3) Ano yung edge case mo? (e.g., qty=10, stock=qty)

### B) Coding check
Create `checks/m02_check.py`:
```py

def discount_amount(subtotal, qty):
    # 5% if qty >= 10 else 0
    pass


def can_sell(qty, stock):
    # return True/False
    pass
```

## 6) Submission
- Branch: `module-02-conditionals`
- PR title: `Module 02 - Discount + Stock Guard`
- Include: one successful run + one out-of-stock run

## 7) Rubric (20 pts)
- (6) correct out-of-stock handling
- (6) correct discount math
- (4) correct totals/change
- (2) clean output
- (2) readable code

## 8) Corrective actions (if <80%)
- If confusion on comparisons: redo micro-drill #1 and #2 with 5 extra test cases.
- If discount wrong: show your formula + compute by hand for 3 cases (qty 9,10,12).
- If type issues: add `try/except` input parsing (optional) and resubmit.
