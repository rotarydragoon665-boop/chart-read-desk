# Chart Read Desk

Snap or upload a TradingView chart and get a day-trade ticket (entry, stop, targets, position size) checked against a rulebook distilled from my Trade notes vault, or a reason to stay flat.

## Use it

1. Open the site (GitHub Pages).
2. Under **Claude connection**, paste an Anthropic API key from https://console.anthropic.com/settings/keys. It is stored only in your browser's local storage and sent only to `api.anthropic.com`.
3. Set your risk rules (equity, risk %, minimum reward:risk, daily loss limit).
4. Take a photo or upload a screenshot and press **Find the trade**.

Charts are read by `claude-opus-5-5`. The page itself computes position size (`equity × risk% ÷ |entry − stop|`), R multiples and the break-even win rate, and forces **NO TRADE** when a rule fails.

Not financial advice. Prices read from a picture can be wrong; check every level on the live chart.
