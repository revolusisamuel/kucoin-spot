# kucoin-spot

> kucoin · spot · paper

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

KuCoin spot paper bot — stub ticker and fills.

## Features

- Default venue kucoin / BTCUSDT
- Built-in ema strategy plus paper mode
- Risk manager with daily-loss kill switch
- OHLCV store and SHA-256 stub candles
- Backtester with fill + fee model
- Click CLI: backtest, paper, status, orders

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd kucoin-spot
python -m pip install -e .
python -m kucoinspot --help
```

## CLI Usage

```bash
kucoinspot backtest --bars 200
# Replay stub candles

kucoinspot paper
# Start a paper session

kucoinspot status
# Print engine state

kucoinspot orders
# List simulated fills
```

## Project Structure

```
kucoinspot/
  core/        engine + risk
  strategy/    grid / dca / ema hooks
  exchange/    stub order client
  data/        candles + backtest
  cli.py
tests/
```

## Configuration

See `kucoinspot/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `exchange` | `kucoin` | Venue id |
| `symbol` | `BTCUSDT` | Default pair |
| `strategy` | `ema` | Active strategy |
| `mode` | `paper` | paper or backtest |

## Tests

```bash
python -m pytest -q
```

## Background

KuCoin Python bots use kucoin-spot as the repo name.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![kucoin](https://img.shields.io/badge/kucoin-111827?style=flat-square) ![spot](https://img.shields.io/badge/spot-111827?style=flat-square) ![kucoin-spot](https://img.shields.io/badge/kucoin%20spot-111827?style=flat-square) ![trading-bot](https://img.shields.io/badge/trading%20bot-111827?style=flat-square) ![crypto-trading](https://img.shields.io/badge/crypto%20trading-111827?style=flat-square) ![binance](https://img.shields.io/badge/binance-111827?style=flat-square) ![defi](https://img.shields.io/badge/defi-111827?style=flat-square) ![algorithmic-trading](https://img.shields.io/badge/algorithmic%20trading-111827?style=flat-square)

`kucoin` `spot` `kucoin-spot` `trading-bot` `crypto-trading` `binance` `defi` `algorithmic-trading` `quantitative-finance` `open-source` `python`

Search: kucoin-spot · kucoin · spot · paper · KuCoin spot paper bot — stub ticker and fills.

---

<sub>KuCoin spot paper bot — stub ticker and fills.</sub>
