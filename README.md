# Aave V2 Wallet Credit Scorer

Assigns credit scores (0–1000) to wallets based on Aave V2 transaction behavior.

## Methodology

We extract wallet behavior features like:
- Interaction types (deposit, borrow, repay, etc.)
- Volume and frequency
- Risk indicators like liquidation count

A Random Forest model is trained using a heuristic score as pseudo-label.

## Architecture
```
[JSON File] → [Preprocess] → [Feature Engineering] → [Model Training] → [Scoring]
```

## To Run
```bash
pip install -r requirements.txt
python src/score_wallets.py data/sample_transactions.json
```

## Output
- `wallet_scores.csv`: Wallet address and credit score between 0–1000
- `distribution.png`: Score distribution graph
