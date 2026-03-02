# Hyperliquid Futures Data for Freqtrade

Daily-updated OHLCV, funding rate, and mark price data for all Hyperliquid futures pairs.

## Data Coverage

- **Exchange:** Hyperliquid (futures)
- **Timeframes:** 1m, 3m, 5m, 15m, 30m, 1h, 2h, 4h, 8h, 12h, 1d, 3d, 1w, 1M
- **Additional:** funding_rate (1h), mark (8h)
- **Pairs:** All listed futures pairs (298+)
- **Format:** Apache Feather files
- **History:** September 2024 onwards

## Usage

Clone with shallow depth for fastest download:

```bash
git clone --depth 1 https://github.com/guibvieira/freqtrade-hyperliquid-data.git
```

Copy data to your Freqtrade installation:

```bash
cp -r freqtrade-hyperliquid-data/user_data/data/hyperliquid /path/to/freqtrade/user_data/data/
```

## Automation

- **Daily download:** GitHub Actions workflow runs at 16:00 UTC
- **Weekly squash:** History is squashed weekly to keep repo size minimal

## Data Size

~2.6 GB total. The 1m timeframe accounts for ~47% of the data.
