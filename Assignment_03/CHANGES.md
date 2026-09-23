# Assignment 03 — CHANGES

**Name:** Phyo Thant Kyaw  **Student ID:** 6705140033

This is the written part of your submission. Explain **what you changed and why**, then record your **prompt log**. Keep before/after snippets to a line or two.

---

## 1 · What I changed

| 1 | Products stored as tuples in the `PRODUCTS` list | `Product` class with `name`, `price`, and `category` | Classes / Composition | Ran `python Assignment_03.py` → PASS |

| 2 | Membership tiers used `if/elif` chains for discount and points | Customer tier classes with separate discount and points behaviour | Inheritance / Polymorphism | Ran `python Assignment_03.py` → PASS |
| 3 | Order items stored as tuples with a product index and quantity | `OrderItem` class with a `Product` object and `quantity` | Composition | Ran `python Assignment_03.py` → PASS |

| 4 | Calculations and receipt printing were mixed inside `calc()` | Separate `subtotal()`, `discount()`, `tax()`, `total()`, `points()`, and `receipt()` methods | Separation of concerns / Pure methods | Ran `python Assignment_03.py` → PASS |

| 5 | Magic numbers and the global `TAXRATE` were used in the calculations | Named constants for tax, discount threshold, bulk discount, and points calculation | Clean code / Encapsulation | Ran `python Assignment_03.py` → PASS |

## 2 · Short reflection (4–6 sentences)

Which change improved the code the most, and why? Where did keeping the behaviour identical force you to be careful?

>Short Reflection

The biggest improvement was changing the tier if/elif statements into different customer classes. It made the code cleaner and easier to understand. Using classes for products and orders also made the code more organized. I had to be careful to keep the same discounts, tax, points, and receipt output. I checked the final code by running python Assignment_03.py and making sure it printed PASS.

---

## 3 · Prompt log (Level 2 — required)

| 1 | "Refactor my messy store system into OOP while keeping the same output." | Suggested Product, OrderItem, Order, and Customer classes | Edited to match my code | Self-test PASS; read every line |

| 2 | "Change the membership tier if/elif statements into OOP." | Suggested separate classes for membership tiers with discount and points behaviour | Edited to fit my code | Self-test PASS; checked discount and points |

| 3 | "Change the product and order item tuples into classes." | Suggested Product and OrderItem objects | Accepted and adjusted | Self-test PASS; checked the output |

| 4 | "Separate the calculations from the receipt printing." | Suggested separate methods for subtotal, discount, tax, total, points, and receipt | Edited to match my code | Self-test PASS; checked the calculations |

| 5 | "Fix the indentation error at def subtotal()." | Suggested correcting the indentation of the method | Accepted | Ran `py Assignment_03.py` → PASS |

**Ownership statement.** *By submitting, I confirm I understand and can explain every line of code I submitted, and that this prompt log reflects my actual AI use.*

---

## 4 · Before-you-submit checklist

- [ ] `python Assignment_03.py` prints **PASS**.
- [ ] No tuples / parallel lists left — products, orders, and items are objects.
- [ ] No `if tier == ...` chains — tiers are a class family.
- [ ] Calculation methods **return** values and do not `print`; printing is separate.
- [ ] Constructors validate state; no leftover `global`; magic numbers are named.
- [ ] The change table and reflection above are filled in.
- [ ] The prompt log is complete and the ownership statement is signed.
