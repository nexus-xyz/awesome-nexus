# Awesome Nexus

[![Discord][discord-badge]][discord-url]
[![X (Twitter)][x-badge]][x-url]

[discord-badge]: https://img.shields.io/badge/Discord-Join%20Chat-blue?style=flat&logo=discord
[discord-url]: https://discord.gg/nexus-xyz
[x-badge]: https://img.shields.io/badge/X-Follow-blue?style=flat&logo=x
[x-url]: https://x.com/nexuslabs

![](./assets/awesome-nexus.png)

A curated list of awesome Nexus resources, tools, and libraries. Inspired by [awesome-go](https://github.com/avelino/awesome-go), [awesome-rust](https://github.com/rust-unofficial/awesome-rust), and other awesome lists.

Nexus is an EVM-compatible Layer 1 blockchain with a powerful zkVM that enables developers to build and deploy applications with ease.

## Contents

- [Awesome Nexus](#awesome-nexus)
  - [Contents](#contents)
  - [Official Resources](#official-resources)
  - [Media](#media)
  - [Nexus Technology](#nexus-technology)
    - [Nexus Layer 1](#nexus-layer-1)
    - [Nexus zkVM](#nexus-zkvm)
    - [Network Services](#network-services)
    - [Nexus OS](#nexus-os)
  - [Developer Resources](#developer-resources)
    - [Network Configuration](#network-configuration)
    - [Testnets](#testnets)
    - [Example Apps](#example-apps)
  - [Research](#research)
    - [Zero-Knowledge Evolution](#zero-knowledge-evolution)
    - [Key Research Papers](#key-research-papers)
    - [Recent Advancements](#recent-advancements)
  - [Ecosystem](#ecosystem)
  - [Call for Projects](#call-for-projects)
    - [Financial Applications](#financial-applications)
    - [AI \& Autonomous Agents](#ai--autonomous-agents)
    - [zkVM Extensions \& Integration](#zkvm-extensions--integration)
    - [Layer-2 \& Layer-3 Solutions](#layer-2--layer-3-solutions)
    - [Social \& Identity](#social--identity)
  - [Contributing](#contributing)

## Official Resources

- [Website](https://nexus.xyz)
- [Documentation](https://docs.nexus.xyz/)
- [GitHub](https://github.com/nexus-xyz)
- [Blog](https://blog.nexus.xyz/)
- [Media](https://nexus.xyz/media) - Videos and presentations, including Stanford lectures
- [Whitepaper](https://whitepaper.nexus.xyz)

## Media

- [Nexus YouTube Channel](https://www.youtube.com/@nexuslabshq) - Official Nexus YouTube account
- [Stanford Seminar - MS&E447: ZKP Panel](https://youtu.be/FAVz5IjyWks?feature=shared) - Panel with Dan Boneh, Jens Groth, Daniel Marin, and Ravi Mhatre
- [Nexus Supercomputer Announcement](https://youtu.be/z8x2n7h40mY?feature=shared) - Introduction to the Nexus Supercomputer
- [Nexus Layer-1 Announcement](https://youtu.be/enwDm_IDk-o?feature=shared) - Launch of the Nexus Layer-1 blockchain
- [Nexus zkVM 2.0 Announcement](https://youtu.be/F8PsoZvrD48?feature=shared) - Introduction to zkVM 2.0 features
- [Nexus zkVM 1.0 Announcement](https://youtu.be/ok7dua_9Jt8?feature=shared) - Launch of the first Nexus zkVM

## Nexus Technology

### Nexus Layer 1

Nexus Layer 1 is a planetary-scale blockchain supercomputer that:

- Concentrates compute power into a single chain
- Scales horizontally with each new node
- Scales vertically with the Nexus zkVM
- Creates a unified proof of all computation: the Proof Singularity

### Nexus zkVM

The Nexus zkVM is a modular, extensible, open-source zkVM written in Rust, focused on performance and security.

**Key Features:**
- Proves any computation with zero-knowledge proofs
- Open source with no proprietary components
- Modular and extensible architecture
- Security-focused design

**Simple Workflow:**
```bash
cargo nexus prove
cargo nexus verify
```

**Evolution of Nexus zkVM:**

| Version | Release | Key Advancements | Performance Gain |
|---------|---------|------------------|-----------------|
| 0.0     | Initial | First general-purpose zkVM | Baseline |
| 1.0     | 2023    | Parallel proving, optimized circuits | 10x |
| 2.0     | 2024    | Multi-core acceleration, specialized hardware | 100x |
| 3.0     | Coming soon | Distributed proving, novel cryptography | 1000x+ |

This exponential improvement represents a new **Moore's Law for verifiable computation**, with each generation delivering order-of-magnitude improvements in proving speed, cost efficiency, and computational capacity.

### Network Services

- [Nexus Explorer](https://explorer.nexus.xyz) - Blockchain explorer
- [Nexus Hub](https://hub.nexus.xyz) - Network dashboard
- [Nexus Status](https://status.nexus.xyz) - Network status
- [Nexus Bridge](https://bridge.nexus.xyz) - Cross-chain bridge
- [NEX Points](https://docs.nexus.xyz/layer-1/nex-points) - Earn points by running nodes

### Nexus OS

Nexus OS provides a unified interface to the Nexus ecosystem across multiple platforms:

- **Web**: [app.nexus.xyz](https://app.nexus.xyz)
- **Mobile**: iOS and Android applications
- **Desktop**: Windows, macOS, and Linux applications

**Key Features:** Wallet management, cross-platform synchronization, dApp discovery, network monitoring, staking, governance, and NEX Points tracking.

Download at [nexus.xyz/download](https://nexus.xyz/download).

## Developer Resources

### Network Configuration

```json
{
  "chainId": "393",
  "rpcUrl": "https://rpc.nexus.xyz/http",
  "wsUrl": "wss://rpc.nexus.xyz/ws",
  "explorerUrl": "https://explorer.nexus.xyz"
}
```

### Testnets

**Testnet II** is the latest Nexus testnet, featuring:
- Enhanced stability and performance
- Full EVM compatibility for seamless Ethereum dApp deployment
- Increased transaction throughput
- Improved developer tooling
- [Testnet Faucet](https://faucet.nexus.xyz) for obtaining test tokens

**Testnet II Configuration:**
```json
{
  "chainId": "393",
  "rpcUrl": "https://testnet-rpc.nexus.xyz/http",
  "wsUrl": "wss://testnet-rpc.nexus.xyz/ws",
  "explorerUrl": "https://testnet-explorer.nexus.xyz"
}
```

### Example Apps

- [Counter App](https://github.com/nexus-xyz/nexus-counter-app) - Simple smart contract demo
- [NFT Platform](https://github.com/nexus-xyz/nexus-nft-example) - NFT creation and trading platform

## Research

### Zero-Knowledge Evolution

**Timeline of Major Developments:**

- **1985**: Introduction of zero-knowledge proofs by Goldwasser, Micali, and Rackoff
- **1988**: First practical zero-knowledge protocols and Fiat-Shamir heuristic
- **1992**: Introduction of probabilistically checkable proofs (PCPs)
- **2010-2012**: Development of zk-SNARKs for practical applications
- **2016**: Zcash launches with zk-SNARKs
- **2019-Present**: Explosion of research in recursive proof systems and zkVMs

### Key Research Papers

**Foundational Theory:**
- ["The Knowledge Complexity of Interactive Proof Systems"](https://people.csail.mit.edu/silvio/Selected%20Scientific%20Papers/Proof%20Systems/The_Knowledge_Complexity_Of_Interactive_Proof_Systems.pdf) (Goldwasser, Micali, Rackoff, 1985)
- ["How to Construct Zero-Knowledge Proof Systems for NP"](https://www.wisdom.weizmann.ac.il/~oded/gmw1.html) (Goldreich, Micali, Wigderson, 1986)
- ["Non-Interactive Zero-Knowledge"](https://link.springer.com/chapter/10.1007/0-387-34805-0_37) (Blum, Feldman, Micali, 1988)

**Modern SNARKs:**
- ["Pinocchio: Nearly Practical Verifiable Computation"](https://eprint.iacr.org/2013/279.pdf) (Parno et al., 2013)
- ["Scalable Zero Knowledge via Cycles of Elliptic Curves"](https://eprint.iacr.org/2014/595.pdf) (Ben-Sasson et al., 2014)
- ["Groth16: On the Size of Pairing-Based Non-interactive Arguments"](https://eprint.iacr.org/2016/260.pdf) (Groth, 2016)

**Transparent Setup Systems:**
- ["Bulletproofs: Short Proofs for Confidential Transactions and More"](https://eprint.iacr.org/2017/1066.pdf) (Bünz et al., 2018)
- ["STARK: Scalable, Transparent ARguments of Knowledge"](https://eprint.iacr.org/2018/046.pdf) (Ben-Sasson et al., 2018)
- ["Halo: Recursive Proof Composition without a Trusted Setup"](https://eprint.iacr.org/2019/1021.pdf) (Bowe et al., 2019)

### Recent Advancements

- **Nova** (2021): ["Nova: Recursive Zero-Knowledge Arguments from Folding Schemes"](https://eprint.iacr.org/2021/370.pdf)
- **Jolt** (2023): ["Jolt: SNARKs for Virtual Machines via Lookups"](https://eprint.iacr.org/2023/1217)
- **HyperNova** (2023): ["HyperNova: Recursive Arguments for Customizable Constraint Systems"](https://eprint.iacr.org/2023/573)
- **STWO** (2023): ["STWO: Short Transparent Witness-Indistinguishable Arguments"](https://eprint.iacr.org/2023/1784)
- **Brakedown** (2023): ["Brakedown: Linear-time Lattice-based Transparent Arguments"](https://eprint.iacr.org/2023/1522)
- **Neo** (2024): ["Neo: Practical Zero-Knowledge Proofs for Ethereum"](https://eprint.iacr.org/2024/035)

## Ecosystem

Nexus is building a robust ecosystem of partners and developers:

- **Advanced R&D Partners**: Collaborations with cryptographers and engineers
- **Strategic Partners**: Organizations exploring applications of verifiable computation
- **Compute Providers**: Contributors to the distributed prover network

To join the Nexus ecosystem, contact [growth@nexus.xyz](mailto:growth@nexus.xyz).

## Call for Projects

We're looking for innovative projects in these key areas:

### Financial Applications
- **DEXs & Aggregators**: High-performance exchanges and routing solutions
- **Stablecoins & Structured Products**: Novel stability mechanisms and yield products
- **Prediction Markets & Derivatives**: Transparent markets with efficient settlement
- **RWA Tokenization**: Infrastructure for traditional asset tokenization
- **Undercollateralized Lending**: Privacy-preserving credit scoring systems

### AI & Autonomous Agents
- **On-Chain AI**: Autonomous agents for strategy execution and asset management
- **Verifiable AI Inference**: zkVM-generated proofs of AI model execution
- **AI-Powered Oracles & Market Makers**: Intelligent data interpretation and liquidity provision

### zkVM Extensions & Integration
- **Language Support & ISAs**: Support for additional languages and architectures
- **Developer Tooling**: IDEs, debuggers, and testing frameworks
- **Frontend Integration**: NextJS/Vercel templates and React component libraries
- **Mobile & Browser Extensions**: Native SDKs and browser extensions

### Layer-2 & Layer-3 Solutions
- **Rollups & Application-Specific Chains**: Specialized chains settling on Nexus
- **Cross-Chain Messaging & Interoperability**: Efficient protocols for asset and data transfer

### Social & Identity
- **Social Graphs & Reputation Systems**: Decentralized networks with verifiable interactions
- **Identity Solutions**: Self-sovereign identity with selective disclosure
- **Social Recovery & Media**: Innovative recovery mechanisms and content platforms

Join our [Discord](https://discord.gg/nexus-xyz) to discuss your ideas or contact [growth@nexus.xyz](mailto:growth@nexus.xyz) for partnership opportunities.

## Contributing

To add your project to this list:

1. Fork this repository
2. Add your project under the appropriate category
3. Submit a pull request with a clear description

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

