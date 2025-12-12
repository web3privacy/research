# Privacy Project Tags

This file documents the tagging methodology used to label `privacy-projects.md` collected from hackathons. Tags reflect three orthogonal dimensions we use across the dataset:

- Use-case / Domain (what the project is for)
- Core Technology (what privacy or building-block tech it uses)
- Tooling / Infra / Region (supporting categories or community focus)

When contributing or reviewing a project, prefer 1–3 primary tags: one use-case tag, one technology tag (if relevant), and up to one tooling/region tag. Extra tags may be added when a project legitimately spans multiple areas (e.g., a privacy wallet that uses ZK and TEE).

---

## Use-Case / Domain Tags (observed in the dataset)

| Tag         | Description |
|-------------|-------------|
| `finance`   | Financial or DeFi applications (private swaps, payments, lending, RWA, escrow) |
| `defi`      | Use-case-focused DeFi primitives (bridges, pools, private trading) — often used alongside `finance` in the data |
| `social`    | Privacy-preserving social platforms, feeds, or community features |
| `ai`        | Projects combining privacy with AI (private ML, agent/ZK integrations) |
| `auth`      | Authentication, age verification, social-login privacy layers, attestations |
| `identity`  | Decentralized identity, anonymous credentials, Sybil-resistance, ZK KYC patterns |
| `wallet`    | Wallet UX, threshold wallets, recovery, private key management |
| `gaming`    | Game mechanics requiring private state (sealed moves, hidden info) |
| `healthcare`| Health or medical-data focused privacy applications |
| `infra`     | Infrastructure, privacy rollups, relayers, or middleware components |
| `security`  | Security-focused tooling: privacy-preserving auditing, post-quantum primitives, secret management |
| `communication` | Encrypted messaging, private content publishing, private email-like flows |
| `dao`       | Private governance, voting, reputation systems for DAOs |
| `reputation`| Reputation and scoring with privacy-preserving properties |
| `analytics` | Privacy-respecting analytics and telemetry approaches |
| `education` | Tutorials, learning tools, onboarding and community education projects |
| `marketplaces` | Marketplaces, private auctions, or commerce flows with confidentiality |
| `music`     | Media/music-specific privacy use-cases |
| `insurance` | Insurance or cyber-insurance infrastructure with confidentiality needs |

---

## Technology Tags (privacy and enabling tech seen in projects)

| Tag      | Description |
|----------|-------------|
| `zk`     | Zero-knowledge proofs (e.g., zk-SNARK, zk-STARK, generic "zk" references) — the single most frequent tech tag in the dataset |
| `ai`     | AI/ML usages (private inference, agent integrations) |
| `tee`    | Trusted Execution Environments and vendor-specific variants (Nitro, TDX, secure enclave mentions) |
| `mpc`    | Secure Multi-Party Computation implementations or protocols |
| `fhe`    | Fully Homomorphic Encryption or related references |
| `semaphore` | Use of Semaphore-like signaling for anonymous group membership |
| `maci`   | MACI-like voting primitives or similar privacy-preserving governance tooling |
| `mixnets`| Mixnets or metadata-mixing approaches (mixers, anonsets) |
| `anonsets`| Ring-signature / anonymity-set techniques (tor/ring references) |

These technology tags are derived from regex-based detection in project descriptions and should be used to indicate the primary privacy technique the project highlights.

---

## Tooling / Dev Infra / Region Tags

 Tag        | Description |
|------------|-------------|
| `tooling`  | SDKs, libraries, or developer tools intended to accelerate private-app development |
| `infra`    | L1/L2s, rollups, relayers, storage or infra-specific components |
| `wallet-fe`| Wallet front-end or UX-specific work (use `wallet` for the broader wallet category) |
| `analytics`| Privacy-preserving analytics, instrumentation or DAQ patterns |
| `education`| Learning or onboarding-focused artifacts |
| `europe`   | Project primarily targeted at or built by EU community |
| `latam`    | Targeted at or built by Latin American community |
| `asia`     | Asia-focused projects |
| `africa`   | Africa-focused projects |

Region tags are optional and were added to reflect community focus in the raw data.

---

## Tagging Guidance (methodology)

- Prefer lowercased, comma-separated tags. Examples: `finance`, `zk`, `infra` or `social`, `zk`, `education`.
- Use 1 primary use-case tag (domain), 0–1 technology tags (if a clear privacy primitive is used), and 0–1 tooling/region tags. Up to 4 tags are allowed when justified.
- When a project mentions multiple privacy technologies, tag the one that is central to the project's privacy claims (or list both if both are central). The dataset's technology counts are approximate and derived from regex matching.
- Avoid overly granular tags for one-off experiments; reserve new tags for repeated or growing patterns.

---

## Examples (mapping real projects to tags)

- LOCUSt (Buenos Aires): `finance`, `zk`, `defi`
- ZKRSS (Buenos Aires): `communication`, `zk`, `infra`
- Void Wallet (Buenos Aires): `wallet`, `zk`
- ProverX (Buenos Aires): `ai`, `zk`, `tooling`
- Private Deals (Buenos Aires): `finance`, `zk`, `infra`

If you think a tag is missing or a mapping is incorrect for a project, propose the change in the dataset's PR with a short justification.

These tags are tuned to the vocabulary and methodology observed in `hackathons.md`, `privacy-projects.md`, and `stats.md`.

Thanks for helping organize the hackathons in the Ethereum privacy ecosystem!
