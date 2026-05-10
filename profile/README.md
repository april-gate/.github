# April Gate

**Tamper-evident cold chain verification for pharmaceutical cargo — powered by Solana.**

Cold chain disputes cost the pharmaceutical industry $35 billion annually. Centralized logs can be altered, backdated, and challenged in court. April Gate replaces thousands of mutable temperature records with a single zero-knowledge proof — recorded permanently on blockchain. Nobody can alter it. Not us, not the shipper, not anyone.

→ [aprilgatehq.com](https://aprilgatehq.com) · [irina@aprilgatehq.com](mailto:irina@aprilgatehq.com)

---

## Repositories

| Repo | Description |
|---|---|
| [coldchain-core](https://github.com/april-gate/coldchain-core) | ZK consensus proof engine · Rust/Bellman · sensor simulation · Actix REST API |
| [coldchain-programs](https://github.com/april-gate/coldchain-programs) | Solana on-chain programs · device registry · proof submission · Anchor + Pinocchio |
| [coldchain-web](https://github.com/april-gate/coldchain-web) | Public website · operator dashboard · shipment verification portal |
| [coldchain-engine](https://github.com/april-gate/coldchain-engine) | Proprietary consensus engine, ZK proof circuits, and hardware firmware · April Gate's core IP (private) |

---

## How It Works

1. **Hardware-signed sensors** — every reading is signed by the device's 
   ATECC608 secure element. The private key is burned into the chip at 
   manufacture and never leaves.

2. **Multi-sensor consensus** — sensors form a local mesh and reach 
   Byzantine-fault-tolerant agreement on each reading, even when offline. 
   No single sensor (or single attacker) can manipulate the record.

3. **Zero-knowledge attestations** — at each reporting interval, sensors 
   generate a ZK proof that confirms conditions stayed within range, without 
   revealing the underlying operational data. Pharma's competitive logistics 
   information stays private.

4. **Decentralized data archival** — full signed readings and consensus 
   results are stored on a decentralized content-addressed storage layer 
   (Filecoin, Arweave, or equivalent), cryptographically bound to the 
   on-chain anchor. Authorized parties can pull the full record; everyone 
   else sees only the proof.

5. **On-chain anchor** — the ZK proof commitment is submitted to Solana. 
   Immutable, timestamped, verifiable by anyone. The single anchor that 
   ties together the sensor readings, the consensus result, and the 
   archival record.
