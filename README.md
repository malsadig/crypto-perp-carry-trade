# Crypto Perpetual Funding Carry

A crypto statistical arbitrage project testing whether perpetual futures funding
payments can support a simple market-neutral carry strategy: long spot crypto,
short the matching perpetual future, and earn funding when the perpetual trades
rich enough to justify the hedge.

This repository contains the research notebook, compact data panels, generated
tables, and chart outputs behind the project report. For the full report, see [https://mossab.dev/funding-carry](https://mossab.dev/funding-carry)

## Reproducing The Notebook

The notebook is designed to run from the repository root or a subfolder. It
loads the compact panels in `data/` and regenerates the CSV and PNG outputs in
`output/`.

```bash
python -m venv .venv
source .venv/bin/activate
pip install pandas numpy matplotlib jupyter
jupyter notebook crypto_perp_funding_carry.ipynb
```

Then run the notebook cells from top to bottom.