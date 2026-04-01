<p align="center">
  <img src="https://img.shields.io/badge/version-0.1.0-00e599?style=flat-square" />
  <img src="https://img.shields.io/badge/license-MIT%20(for%20now)-7c5cff?style=flat-square" />
  <img src="https://img.shields.io/badge/compliance-vibes--based-ffd700?style=flat-square" />
  <img src="https://img.shields.io/badge/jurisdictions%20violated-47-ff4466?style=flat-square" />
  <img src="https://img.shields.io/badge/SEC%20inquiries-pending-ff4466?style=flat-square" />
</p>

<h1 align="center">⚖️ OmniExchange</h1>

<p align="center">
  <strong>The open-source universal trading platform.</strong><br>
  Securities. Crypto. Prediction markets. Real estate. Horse racing. Riverboat gambling.<br>
  One API. Every asset class. Zero regulatory approval.
</p>

---

## Why OmniExchange?

Modern finance is fragmented. You need one broker for stocks, another for crypto, a third for prediction markets, a bookie for the horses, and a fake mustache to board the riverboat.

**OmniExchange unifies all of this into a single, deployable exchange** that you can run from your laptop, a cloud instance, or an actual boat in international waters.

```
npx create-omni-exchange my-totally-legal-exchange
```

## Quick Start

```typescript
import { OmniExchange } from 'omni-exchange';

const exchange = new OmniExchange({
  name: 'My Totally Legal Exchange',
  assets: ['securities', 'crypto', 'predictions', 'horses', 'riverboat'],
  compliance: 'vibes',           // 'strict' | 'relaxed' | 'vibes' | 'none'
  jurisdiction: 'international-waters',
  maxLeverage: Infinity,         // go big or go home
});

exchange.listen(3000);
console.log('🎰 Exchange is live. Lawyers on standby.');
```

## Supported Asset Classes

| Class | Status | Description |
|-------|--------|-------------|
| 📈 **Securities** | ✅ Live | Stocks, bonds, ETFs, options. Full NBBO compliance (probably). |
| 🪙 **Cryptocurrency** | ✅ Live | 10,000+ tokens. 47 dog-themed coins. Self-custody or YOLO custody. |
| 🎲 **Prediction Markets** | ✅ Live | Bet on anything. Will aliens visit by 2027? Is a hot dog a sandwich? |
| 🏠 **Real Estate** | 🧪 Beta | Fractionalized property. Own 0.003% of a Malibu beach house. |
| 🏇 **Horse Racing** | 🧪 Beta | Algorithmic handicapping meets DeFi. Short a horse. Long the jockey. |
| 🚢 **Riverboat Gambling** | ⚠️ Grey Area | Full casino ops on international waters. Tokenized on-chain. |
| 🎨 **Fine Art** | 🔜 Soon | Fractional Picassos and rare Pokémon cards. |
| 🦁 **Exotic Derivatives** | 🔜 Soon | Weather futures, celebrity reputation swaps, vibes-based indices. |

## Features

- **Sub-millisecond order matching** — 2M orders/sec. Horses matched at a more leisurely pace.
- **Cross-asset atomic swaps** — Sell AAPL, buy a racehorse, hedge with weather futures. One transaction.
- **Compliance-as-a-Spectrum™** — From SEC-grade KYC to "don't ask, don't tell." Per-asset configuration.
- **Jurisdiction Shopping** — Auto-route orders through the most permissive regulatory environment.
- **AI Market Maker** — LLM-powered market making. It doesn't understand finance, but neither do most market makers.
- **One-click deploy** — AWS, GCP, Azure, or an actual boat. Maritime deployment guide included.

## Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    OmniExchange Core                     │
├──────────┬──────────┬──────────┬──────────┬─────────────┤
│Securities│  Crypto  │Prediction│  Horses  │  Riverboat  │
│  Engine  │  Engine  │  Engine  │  Engine  │   Engine    │
├──────────┴──────────┴──────────┴──────────┴─────────────┤
│              Unified Order Book (UOB™)                   │
├─────────────────────────────────────────────────────────┤
│         Compliance Layer (configurable: vibes)           │
├─────────────────────────────────────────────────────────┤
│    Settlement: T+0 (crypto) | T+2 (stocks) | T+🤷 (horses)   │
└─────────────────────────────────────────────────────────┘
```

## Cross-Asset Trading Example

```typescript
// The trade your financial advisor warned you about
await exchange.atomicSwap({
  sell: { asset: '$AAPL', qty: 100 },
  buy: [
    { asset: '$HORSE:THUNDERLEG', qty: 1 },
    { asset: '$PRED:HOTDOGSANDWICH', side: 'YES', qty: 500 },
    { asset: '$RE:MALIBU-4BD', fraction: 0.003 },
    { asset: '$BOAT:BLACKJACK', bet: 'hit-me', qty: 1 },
  ],
  compliance: 'vibes',
});
```

## Deployment Options

| Target | Command | Notes |
|--------|---------|-------|
| Local | `omni up` | For development and light felonies |
| AWS | `omni deploy --aws` | Auto-configures in us-east-1 |
| International Waters | `omni deploy --maritime` | Requires boat. GPS spoofing optional. |
| The Moon | `omni deploy --lunar` | Truly beyond all jurisdiction |

## Configuration

```yaml
# omni.config.yml
exchange:
  name: "Definitely Not A Ponzi"

markets:
  securities:
    enabled: true
    compliance: strict    # we're not animals
  crypto:
    enabled: true
    compliance: relaxed   # okay maybe a little
  predictions:
    enabled: true
    compliance: vibes     # it's fine
  horses:
    enabled: true
    compliance: none      # let them run
  riverboat:
    enabled: true
    compliance: ¯\_(ツ)_/¯
    gps_spoofing: false   # please set to true before launch
```

## Benchmarks

```
Exchange Throughput Test — M1 MacBook Pro
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Stock orders:      2,147,483 ops/sec    ✅
Crypto swaps:      1,842,901 ops/sec    ✅
Horse bets:              847 ops/sec    🐴 (limited by horse speed)
Riverboat hands:       1,200 ops/sec    🃏
Prediction bets:   1,100,420 ops/sec    ✅
Cross-asset swap:    420,069 ops/sec    🔥 nice
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

## FAQ

**Is this legal?**
Depends on where you deploy. Our maritime deployment guide exists for a reason.

**Can I actually make money?**
Theoretically yes. Practically, you'll probably just make the news.

**What about KYC/AML?**
We support full KYC/AML when `compliance` is set to `strict`. We also support `vibes`.

**My horse lost. Can I get a refund?**
No. But you can short the horse retroactively if you enable `temporal_trading` (experimental).

**Do you have a token?**
$OMNI launches Q3 2026. Tokenomics: 40% team, 30% community, 20% horses, 10% legal defense fund.

**Is the riverboat real?**
The riverboat is a state of mind. Also yes, there is a boat.

## Community

- 💬 [Discord](https://discord.gg/fake-link) — 12,000+ members. Active horse racing channel.
- 🐦 [@OmniExchange](https://twitter.com/fake-link) — Market commentary and SEC subpoena updates.
- 📖 [Documentation](https://omni-exchange.dev/fake-link) — Comprehensive guides including maritime law basics.

## Contributing

We welcome contributions! Areas of particular need:

- Maritime law expertise
- Horse whispering algorithms
- Compliance engineers willing to look the other way
- Someone who actually understands how bonds work

See [CONTRIBUTING.md](./CONTRIBUTING.md) for guidelines.

## Legal Disclaimer

```
OmniExchange is provided "AS IS" without warranty of any kind.
The maintainers are not responsible for:
  - Financial losses
  - Regulatory enforcement actions
  - Horse-related injuries (emotional or physical)
  - Maritime incidents
  - Any situation requiring the phrase "I'd like to speak to my lawyer"

By using this software you acknowledge that you have read this
disclaimer and have chosen to proceed anyway, which honestly
says more about you than it does about us.
```

## License

MIT — for now. Subject to change based on ongoing legal proceedings.

---

<p align="center">
  <strong>🎪 Happy April Fools' Day 2026</strong><br>
  <em>Please don't actually build a stock exchange. Or a riverboat casino. Especially not both.</em><br><br>
  Built with questionable judgment by <a href="https://rob-simon.com">Rob Simon</a>
</p>
