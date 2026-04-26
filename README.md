# April Gate

**Tamper-evident cold chain verification for pharmaceutical cargo — powered by Solana.**

Cold chain disputes cost the pharmaceutical industry $35 billion annually. Centralized logs can be altered, backdated, and challenged in court. April Gate replaces thousands of mutable temperature records with a single zero-knowledge proof — recorded permanently on blockchain. Nobody can alter it. Not us, not the shipper, not anyone.

→ [aprilgatehq.com](https://aprilgatehq.com) · [irina@aprilgatehq.com](mailto:irina@aprilgatehq.com)

---

## Repositories

| Repo | Description |
|---|---|
| [coldchain-core](https://github.com/april-gate/coldchain-core) | ZK consensus proof engine · Rust/Bellman · sensor simulation · Actix REST API |
| [coldchain-programs](https://github.com/april-gate/coldchain-programs) | Solana on-chain programs · device registry · proof submission |
| [coldchain-web](https://github.com/april-gate/coldchain-web) | Public website · operator dashboard · shipment verification portal |

---

## How It Works

1. **Hardware-signed sensors** — ATECC608 secure element signs every reading. Private key never leaves the chip.
2. **Multi-sensor consensus** — sensors form a local mesh and agree on readings, even during connectivity dead zones.
3. **Zero-knowledge proof** — a single mathematical certificate proves conditions were valid without revealing operational details.
4. **On-chain record** — proof submitted to Solana. Immutable, verifiable by anyone, forever.

