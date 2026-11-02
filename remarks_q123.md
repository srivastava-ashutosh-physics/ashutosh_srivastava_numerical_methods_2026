# Ashutosh Srivastava

## Question 1 — GitHub and submission (3 marks)

| Section | Marks | Comment |
|---|---:|---|
| Q1 | 2/3 | |

## Question 2 — Binary and IEEE floating-point representation (24 marks)

| Section | Marks | Comment |
|---|---:|---|
| Q2.1 — Decimal integer to binary | 5/5 | |
| Q2.2 — Decimal to IEEE double representation | 5.5/10 | The function handles ordinary finite values, but the zero case returns a 32-bit string rather than the required 64-bit representation. It also lacks handling for infinities, NaN, and subnormal values. The output components include extra labels instead of returning only the bit strings, and the mantissa is truncated rather than rounded. |
| Q2.3 — IEEE representation to decimal | 4.5/5 | The conversion handles normal and subnormal values, zero, infinities, and NaN. A small deduction for not validating the required IEEE double field lengths. |
| Q2.4 — Verification using 200.0, π, +∞ and −∞ | 4/4 | |
| **Q2 Total** | **19/24** | |

## Question 3 — Floating-point error accumulation (16 marks)

| Section | Marks | Comment |
|---|---:|---|
| Q3.1(a) — Grid generation using method1 | 2/2 | |
| Q3.1(b) — Grid generation using method2 | 2/2 | |
| Q3.2(a) — Analytical average | 2/2 | |
| Q3.2(b) — Average using method1 | 2/2 | |
| Q3.2(c) — Average using method2 | 2/2 | |
| Q3.3 — Error calculation and plotting | 4/4 | |
| Q3.4 — Comparison of accuracy | 1.5/2 | The explanation correctly identifies cumulative rounding error in the recurrence method, but the claim that the direct method's errors are strictly bounded near machine precision is too strong without qualification. |
| **Q3 Total** | **15.5/16** | |

## Final

- **Q1:** 2/3
- **Q2:** 19/24
- **Q3:** 15.5/16
- **Overall:** **36.5/43**
