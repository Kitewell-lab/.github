<p align="center">
  <img src="logo.png" width="120" alt="Kitewell logo" />
</p>

<h1 align="center">Kitewell</h1>

<p align="center">
  Wallet tooling for <strong>Stellar Testnet</strong>.
</p>

<p align="center">
  <img src="banner.png" alt="Kitewell" width="100%" />
</p>

Kitewell is a small Stellar stack for trying real wallet flows on Testnet: connect [Freighter](https://www.freighter.app/), fund an account, manage trustlines, send XLM, and read payment history. An API in front of Horizon keeps the UI off the raw network, and a Soroban contract stores optional on-chain check-ins.

Signing never leaves Freighter. The backend does not handle secret keys. Default network is Testnet.

## Repositories

| | Repo | What it does |
|---|------|----------------|
| App | [frontend](https://github.com/Kitewell-lab/frontend) | React + Vite wallet UI |
| API | [backend](https://github.com/Kitewell-lab/backend) | Horizon account and payment reads |
| Contract | [contract](https://github.com/Kitewell-lab/contract) | Soroban registry |

## Run locally

```bash
git clone https://github.com/Kitewell-lab/backend.git
cd backend && npm install && npm run dev

git clone https://github.com/Kitewell-lab/frontend.git
cd frontend && npm install && npm run dev
```

Open http://localhost:5173 with Freighter set to Testnet.

## License

MIT. Testnet only by default.
