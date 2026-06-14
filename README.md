# iso-xmm interface

Public **interface** for the iso-xmm AMM on Solana mainnet, for explorers and aggregators.

- `xmm.json` — the program IDL: the **public, permissionless** instruction surface (swaps and the
  full LP position lifecycle), plus every account, type, and error those instructions reference.
  Operator-only instructions (pool creation for the oracle-anchored maker, pricer updates, inventory
  moves, status/teardown, config) are intentionally **not** published; they require a privileged
  signer and are not callable by integrators.
- `metadata.json` — program name, logo, IDL URL (for the on-chain program-metadata account).
- `mbco-logo.png` — the program logo.

This repo contains **no program source**. iso-xmm is proprietary MBCO code; only the public
interface (which integrators need anyway) is published here.

- Program: `isogrRJ6sEiktnfUY7QdZhDr5Sut3C8ER9HejjUqSZK`
- App: https://xmm.mbco.io
- Integrate: https://xmm.mbco.io/docs
