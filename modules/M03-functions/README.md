# Module 03 — Functions (TPP Store: Reusable Checkout Engine)

## 0) Py4E alignment
- Chapter 4: Functions
- Concepts: `def`, parameters, return values, decomposition

## 1) Learning outcomes (Taglish)
After this module, kaya mo na:
- gumawa ng functions na reusable
- mag-return ng computed values
- mag-break ng malaking problem into smaller steps

## 2) Lesson (short)
**Big idea:** Functions = named steps para hindi repeat at mas madaling i-test.

Common mistakes:
- forgetting `return`
- printing inside a function when you need a value

## 3) Micro-drills
1) `add_tax(amount, rate)`
2) `to_money(x)` returns formatted string with 2 decimals
3) `is_bulk(qty)` returns True if qty >= 10

## 4) Lab — Feature: Checkout functions
### User story
As a cashier, I want a checkout that uses functions so we can extend later (loops/files).

### Requirements
Refactor your Module 02 solution into functions:
- `compute_subtotal(price, qty)`
- `compute_discount(subtotal, qty)`
- `compute_total(subtotal, discount)`
- `compute_change(total, cash)`
- `can_sell(qty, stock)`
- `print_receipt(...)` (prints receipt)

Program flow:
- read inputs
- validate stock via `can_sell`
- compute values via functions
- print receipt

### Constraints
- Still no loops.

## 5) Mastery Gate (80%)
### A) Reflection (PR description)
1) Bakit mas ok ang functions kaysa copy-paste logic?
2) Ano ang difference ng parameter vs argument?
3) Paano mo i-test ang `compute_discount()` without running the whole program?

### B) Coding check
Create `checks/m03_check.py`:
```py

def compute_discount(subtotal, qty):
    # 5% if qty >= 10 else 0
    pass


def compute_change(total, cash):
    pass
```
Plus: add 3 simple asserts in the file:
```py
assert compute_discount(100, 10) == 5
assert compute_discount(100, 9) == 0
assert compute_change(22.8, 50) == 27.2
```

## 6) Submission
- Branch: `module-03-functions`
- PR title: `Module 03 - Functions Checkout Engine`
- Include: one run screenshot + mention which functions you added

## 7) Rubric (25 pts)
- (10) correctness (same outputs as M02)
- (7) good decomposition (right functions, minimal duplication)
- (4) readability/naming
- (4) mastery gate quality

## 8) Corrective actions (if <80%)
- If returns are wrong: rewrite functions to return values only (no prints) except `print_receipt`.
- If output differs: add 3 test cases in `m03_check.py` and show expected vs actual.
