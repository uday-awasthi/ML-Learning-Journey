# Day 37 - Handling Missing Categorical Data

This notebook covers two common techniques for handling missing values in categorical columns.

## Topics Covered

### 1. Most Frequent (Mode) Imputation
- Missing values are replaced with the **most frequent value (mode)** of that column
- Simple and fast technique, useful when missing data is low and one category is already dominant
- Downside: if missing values are large in number, it further inflates the dominant category and can distort the data distribution

### 2. Missing Category Imputation
- Missing values are replaced with a new label like `"Missing"` or `"Unknown"`
- No information is lost — the model can learn that the value was missing
- Useful when the missingness itself carries meaningful information (MNAR - Missing Not At Random)

## Comparison
| Technique | When to use | Risk |
|---|---|---|
| Mode Imputation | When missing values are few | Can bias the distribution |
| Missing Category | When missingness is informative | Adds an extra category |


## References
https://www.youtube.com/watch?v=l_Wip8bEDFQ&list=PLKnIA16_Rmvbr7zKYQuBfsVkjoLcJgxHH&index=37
