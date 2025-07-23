# Aave Credit Score Analysis

## Score Distribution

The model scored wallets between 0 and 1000. Here's the histogram:

![Score Distribution](distribution.png)

| Score Range | # Wallets | Characteristics |
|-------------|-----------|-----------------|
| 0–100       | High liquidation, frequent borrowing without repay |
| 100–200     | Infrequent interaction, moderate borrowing |
| 200–400     | Basic activity, neutral usage |
| 400–700     | Balanced deposits, occasional borrows, repayments seen |
| 700–900     | High deposits, low borrow, consistent use |
| 900–1000    | Frequent use, responsible repay behavior, no liquidation |

## Behavior Insights

- **Low Score Wallets**: Borrow aggressively, high liquidation, lack repayment
- **High Score Wallets**: Frequent deposits, consistent repays, rarely liquidated
