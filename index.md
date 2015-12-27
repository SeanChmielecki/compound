---
title       : Compound Interest Calculator
subtitle    : 
author      : Kevin Wu
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
github      :
    user    : kevinwu6
    repo    : compound
---

## Compound Interest

**Compound interest** is the interest calculated on an initial principal deposit or loan *plus* accumulated interest.

1. The principal amount grows faster than with simple interest.
2. The higher the number of compounding periods, the greater the compound interest.
3. The rate depends on the frequency of compounding.

---

## Compound Interest Calculator

The **Compound Interest Calculator** app allows you to calculate compound interest based on your input:

* Principal Amount
* Annual Interest Rate
* Time Period (assuming annual compounding)

The resulting calculation is the total future value of the deposit or loan — the principal amount plus compound interest.

---

## Benefits

This app will benefit you because.

1. Won't have to perform manual calculations.
2. No need to memorize the formula. Just plug in the numbers and go.
3. Can use as a savings tool — see how much your money will be worth.

---

## Calculator Function

This is the formula that is used.

$$Future\ Value = Principal \times (1 + Rate)^{Time}$$'

This is the code that is run when you hit the "submit" button.


```r
future_value <- function(principal, rate, time) {
    principal * (1 + rate / 100)^(time)
}
```

---

## Example

Now we can test out the function using these values.


```r
principal <- 10000
rate <- 3.875
time <- 5

future_value(principal, rate, time)
```

```
## [1] 12093.59
```

---
