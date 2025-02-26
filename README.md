# Awesome Nexus

[![Discord][discord-badge]][discord-url]
[![X (Twitter)][x-badge]][x-url]

[discord-badge]: https://img.shields.io/badge/Discord-Join%20Chat-blue?style=flat&logo=discord
[discord-url]: https://discord.gg/nexus-xyz
[x-badge]: https://img.shields.io/badge/X-Follow-blue?style=flat&logo=x
[x-url]: https://x.com/nexuslabs

![](./assets/awesome-nexus.png)

A curated list of awesome Nexus resources, tutorials, tools and libraries. Inspired by [awesome-go](https://github.com/avelino/awesome-go), [awesome-rust](https://github.com/rust-unofficial/awesome-rust), [awesome-solidity](https://github.com/bkrem/awesome-solidity), and [awesome-react](https://github.com/enaqx/awesome-react).

Nexus is an EVM-compatible Layer 1 blockchain with a powerful zkVM that enables developers to build and deploy applications with ease.

## Content

- [Awesome Nexus](#awesome-nexus)
  - [Content](#content)
  - [Official Resources](#official-resources)
  - [Nexus Layer 1](#nexus-layer-1)
    - [Network Configuration](#network-configuration)
  - [Nexus zkVM](#nexus-zkvm)
    - [The Evolution of Verifiable Computation](#the-evolution-of-verifiable-computation)
      - [Nexus zkVM Versions](#nexus-zkvm-versions)
  - [Zero-Knowledge Research](#zero-knowledge-research)
    - [History of Zero-Knowledge Proofs](#history-of-zero-knowledge-proofs)
    - [Key Research Papers](#key-research-papers)
    - [Recent Advancements](#recent-advancements)
  - [Nexus Testnets](#nexus-testnets)
    - [Testnet II](#testnet-ii)
  - [Nexus OS](#nexus-os)
  - [Network](#network)
  - [Ecosystem](#ecosystem)
  - [Example Apps](#example-apps)
  - [Call for Startups \& Projects](#call-for-startups--projects)
    - [Financial Applications](#financial-applications)
    - [AI \& Autonomous Agents](#ai--autonomous-agents)
    - [zkVM Extensions \& Tooling](#zkvm-extensions--tooling)
    - [Frontend \& Integration](#frontend--integration)
    - [Layer-2 \& Layer-3 Solutions](#layer-2--layer-3-solutions)
    - [Social \& Identity](#social--identity)
  - [How to Add Your Project](#how-to-add-your-project)

## Official Resources

- [Website](https://nexus.xyz)
- [Documentation](https://docs.nexus.xyz/)
- [GitHub](https://github.com/nexus-xyz)
- [Blog](https://blog.nexus.xyz/)
- [Whitepaper](https://whitepaper.nexus.xyz)

## Nexus Layer 1

The Nexus Layer 1 is a planetary-scale blockchain supercomputer that:

- Concentrates compute power into a single chain
- Scales horizontally with each new node
- Scales vertically with the Nexus zkVM
- Creates a unified proof of all computation: the Proof Singularity

### Network Configuration

```json
{
  "chainId": "393",
  "rpcUrl": "https://rpc.nexus.xyz/http",
  "wsUrl": "wss://rpc.nexus.xyz/ws",
  "explorerUrl": "https://explorer.nexus.xyz"
}
```

## Nexus zkVM

The Nexus zkVM is a modular, extensible, open-source zkVM written in Rust, focused on performance and security.

Key features:
- Proves any computation with zero-knowledge proofs
- Open source with no proprietary components
- Modular and extensible architecture
- Security-focused design

Simple proving workflow:

```bash
cargo nexus prove
cargo nexus verify
```

### The Evolution of Verifiable Computation

Nexus is pioneering the development of general-purpose verifiable compute models through its zkVM evolution:

#### Nexus zkVM Versions

| Version | Release | Key Advancements | Performance Gain |
|---------|---------|------------------|-----------------|
| 0.0     | Initial | First general-purpose zkVM | Baseline |
| 1.0     | 2023    | Parallel proving, optimized circuits | 10x |
| 2.0     | 2024    | Multi-core acceleration, specialized hardware support | 100x |
| 3.0     | Coming soon | Distributed proving, novel cryptographic primitives | 1000x+ |

This exponential performance improvement represents a new type of **Moore's Law for verifiable computation**. While traditional computing follows Moore's Law of doubling transistor density approximately every two years, Nexus's zkVM technology is advancing at an even more accelerated pace, with each generation delivering order-of-magnitude improvements in proving speed, cost efficiency, and computational capacity.

These advancements are enabling entirely new categories of applications that were previously impractical due to performance constraints, from real-time verifiable AI inference to complex financial systems with instant settlement and verification.

## Zero-Knowledge Research

### History of Zero-Knowledge Proofs

Zero-knowledge proofs (ZKPs) represent one of the most significant breakthroughs in modern cryptography, enabling one party to prove to another that a statement is true without revealing any additional information beyond the validity of the statement itself.

**Timeline of Major Developments:**

- **1985**: The concept of zero-knowledge proofs is introduced by Shafi Goldwasser, Silvio Micali, and Charles Rackoff in their seminal paper ["The Knowledge Complexity of Interactive Proof Systems"](https://people.csail.mit.edu/silvio/Selected%20Scientific%20Papers/Proof%20Systems/The_Knowledge_Complexity_Of_Interactive_Proof_Systems.pdf).

- **1988**: The first practical zero-knowledge protocols are developed, including the Fiat-Shamir heuristic for converting interactive proofs to non-interactive ones.

- **1992**: Introduction of probabilistically checkable proofs (PCPs), laying groundwork for future successes in verifiable computation.

- **2010-2012**: Development of zk-SNARKs (Zero-Knowledge Succinct Non-Interactive Arguments of Knowledge), making ZKPs more practical for real-world applications.

- **2016**: Zcash launches as the first widespread application of zk-SNARKs in a cryptocurrency.

- **2019-Present**: Explosion of research in recursive proof systems, transparent setups, and performance optimizations leading to practical zkVMs.

### Key Research Papers

The following papers represent foundational and cutting-edge research in zero-knowledge proofs and verifiable computation:

- **Foundational Theory**:
  - ["The Knowledge Complexity of Interactive Proof Systems"](https://people.csail.mit.edu/silvio/Selected%20Scientific%20Papers/Proof%20Systems/The_Knowledge_Complexity_Of_Interactive_Proof_Systems.pdf) (Goldwasser, Micali, Rackoff, 1985)
  - ["How to Construct Zero-Knowledge Proof Systems for NP"](https://www.wisdom.weizmann.ac.il/~oded/gmw1.html) (Goldreich, Micali, Wigderson, 1986)
  - ["Non-Interactive Zero-Knowledge"](https://link.springer.com/chapter/10.1007/0-387-34805-0_37) (Blum, Feldman, Micali, 1988)

- **Modern SNARKs**:
  - ["Pinocchio: Nearly Practical Verifiable Computation"](https://eprint.iacr.org/2013/279.pdf) (Parno et al., 2013)
  - ["Scalable Zero Knowledge via Cycles of Elliptic Curves"](https://eprint.iacr.org/2014/595.pdf) (Ben-Sasson et al., 2014)
  - ["Groth16: On the Size of Pairing-Based Non-interactive Arguments"](https://eprint.iacr.org/2016/260.pdf) (Groth, 2016)

- **Transparent Setup Systems**:
  - ["Bulletproofs: Short Proofs for Confidential Transactions and More"](https://eprint.iacr.org/2017/1066.pdf) (Bünz et al., 2018)
  - ["STARK: Scalable, Transparent ARguments of Knowledge"](https://eprint.iacr.org/2018/046.pdf) (Ben-Sasson et al., 2018)
  - ["Halo: Recursive Proof Composition without a Trusted Setup"](https://eprint.iacr.org/2019/1021.pdf) (Bowe et al., 2019)

### Recent Advancements

Recent breakthroughs have dramatically improved the efficiency and practicality of zero-knowledge systems:

- **Nova** (2021): ["Nova: Recursive Zero-Knowledge Arguments from Folding Schemes"](https://eprint.iacr.org/2021/370.pdf)
  - Introduces a folding scheme for recursive proof composition with logarithmic verification time
  - Enables practical recursive SNARKs without trusted setup

- **Jolt** (2023): ["Jolt: SNARKs for Virtual Machines via Lookups"](https://eprint.iacr.org/2023/1217)
  - Achieves significant performance improvements for zkVMs through optimized lookup arguments
  - Reduces proof generation time by orders of magnitude

- **HyperNova** (2023): ["HyperNova: Recursive Arguments for Customizable Constraint Systems"](https://eprint.iacr.org/2023/573)
  - Extends Nova with support for customizable constraint systems
  - Enables more efficient proofs for complex computations

- **STWO** (2023): ["STWO: Short Transparent Witness-Indistinguishable Arguments"](https://eprint.iacr.org/2023/1784)
  - Provides short transparent witness-indistinguishable arguments
  - Achieves significant improvements in proof size and verification time

- **Brakedown** (2023): ["Brakedown: Linear-time Lattice-based Transparent Arguments"](https://eprint.iacr.org/2023/1522)
  - Introduces linear-time lattice-based transparent arguments
  - Offers post-quantum security properties

- **Neo** (2024): ["Neo: Practical Zero-Knowledge Proofs for Ethereum"](https://eprint.iacr.org/2024/035)
  - Optimized for Ethereum's execution environment
  - Achieves significant gas savings for on-chain verification

These advancements form the foundation of Nexus's zkVM technology, with each generation incorporating the latest research to deliver exponential performance improvements.

## Nexus Testnets

Nexus operates a series of testnets to allow developers to experiment and build applications in a safe environment before deploying to mainnet.

### Testnet II

Testnet II is the latest Nexus testnet, featuring:

- Enhanced stability and performance
- Full EVM compatibility for seamless Ethereum dApp deployment
- Increased transaction throughput
- Improved developer tooling and support
- Faucet for obtaining test tokens: [Testnet Faucet](https://faucet.nexus.xyz)

To connect to Testnet II, use the following configuration:

```json
{
  "chainId": "393",
  "rpcUrl": "https://testnet-rpc.nexus.xyz/http",
  "wsUrl": "wss://testnet-rpc.nexus.xyz/ws",
  "explorerUrl": "https://testnet-explorer.nexus.xyz"
}
```

Join the [Discord](https://discord.gg/nexus-xyz) to get support and connect with other developers building on Testnet II.

## Nexus OS

Nexus OS is a multi-platform operating system for interacting with the Nexus ecosystem, available across:

- **Web**: Access the full Nexus experience through any modern web browser at [app.nexus.xyz](https://app.nexus.xyz)
- **Mobile**: Native iOS and Android applications providing on-the-go access to the Nexus network
- **Desktop**: Dedicated applications for Windows, macOS, and Linux with enhanced functionality

Key features of Nexus OS:

- Unified wallet management
- Cross-platform synchronization
- dApp discovery and interaction
- Network monitoring and analytics
- Staking and governance participation
- NEX Points tracking and rewards

Download Nexus OS for your platform at [nexus.xyz/download](https://nexus.xyz/download).

## Network

- [Nexus Explorer](https://explorer.nexus.xyz) - Blockchain explorer
- [Nexus Hub](https://hub.nexus.xyz) - Network dashboard
- [Nexus Status](https://status.nexus.xyz) - Network status
- [Nexus Bridge](https://bridge.nexus.xyz) - Cross-chain bridge
- [NEX Points](https://docs.nexus.xyz/layer-1/nex-points) - Earn points by running nodes

## Ecosystem

Nexus is building a robust ecosystem of partners and developers advancing verifiable computation:

- **Advanced R&D Partners**: Collaborations with cryptographers and engineers
- **Strategic Partners**: Organizations exploring new applications of verifiable computation
- **Compute Providers**: Contributors to the distributed prover network

To join the Nexus ecosystem, contact [growth@nexus.xyz](mailto:growth@nexus.xyz).

## Example Apps

- [Counter App](https://github.com/nexus-xyz/nexus-counter-app) - Simple counter application demonstrating basic smart contract functionality
- [NFT Platform](https://github.com/nexus-xyz/nexus-nft-example) - NFT platform showcasing creation, trading, and management

## Call for Startups & Projects

We're looking for innovative projects to build on Nexus across several key areas:

### Financial Applications
- **Decentralized Exchanges (DEXs)**: Build high-performance, low-slippage DEXs leveraging Nexus's speed and security
- **DEX Aggregators**: Create optimized routing solutions across multiple liquidity sources
- **Stablecoins**: Develop algorithmic or collateralized stablecoins with novel stability mechanisms
- **Prediction Markets**: Build markets for forecasting events with transparent resolution via zkProofs
- **Structured Products**: Create yield-generating products with verifiable risk profiles
- **Options & Derivatives**: Develop on-chain options and derivatives markets with efficient settlement
- **Real-World Asset (RWA) Tokenization**: Build infrastructure for tokenizing and trading traditional assets
- **Undercollateralized Lending**: Create reputation-based lending protocols with privacy-preserving credit scoring

### AI & Autonomous Agents
- **On-Chain AI Agents**: Deploy autonomous AI agents that can execute strategies and manage assets
- **Verifiable AI Inference**: Use the zkVM to generate proofs of AI model execution and results
- **Decentralized Machine Learning**: Build collaborative learning systems with verifiable computation
- **AI-Powered Oracles**: Create intelligent oracles that can interpret complex real-world data
- **Autonomous Market Makers**: Develop AI-driven liquidity provision strategies
- **Agent-Based Governance**: Build governance systems with AI agents representing stakeholder interests

### zkVM Extensions & Tooling
- **Language Support**: Extend the zkVM to support additional programming languages beyond Rust
- **Instruction Set Architectures**: Add support for new ISAs to broaden compatibility
- **Prover Architectures**: Develop specialized provers optimized for specific computation types
- **Developer Tooling**: Create IDEs, debuggers, and testing frameworks for zkVM development
- **Precompiles & Libraries**: Build optimized precompiles for common cryptographic operations
- **Benchmarking Tools**: Develop tools to measure and optimize zkVM performance

### Frontend & Integration
- **NextJS Integration**: Create starter kits and libraries for seamless Nexus integration with NextJS
- **Vercel Deployment Templates**: Develop templates for one-click deployment of Nexus dApps on Vercel
- **React Component Libraries**: Build UI component libraries specifically for Nexus applications
- **Mobile SDK**: Develop SDKs for native mobile integration with iOS and Android
- **Browser Extensions**: Create browser extensions for seamless interaction with Nexus

### Layer-2 & Layer-3 Solutions
- **Rollups Settling on Nexus**: Build optimistic or ZK rollups using Nexus as a settlement layer
- **Application-Specific Chains**: Develop specialized chains for specific use cases that settle on Nexus
- **Cross-Chain Messaging**: Create efficient messaging protocols between Nexus and other chains
- **Data Availability Solutions**: Build data availability layers optimized for Nexus
- **Interoperability Protocols**: Develop bridges and protocols for seamless asset and data transfer

### Social & Identity
- **Social Graphs**: Build decentralized social networks with verifiable interactions
- **Reputation Systems**: Create on-chain reputation systems with privacy-preserving features
- **Identity Solutions**: Develop self-sovereign identity frameworks with selective disclosure
- **Social Recovery**: Build innovative account recovery mechanisms using social connections
- **Decentralized Social Media**: Create platforms for content sharing with fair creator compensation

Join our [Discord](https://discord.gg/nexus-xyz) to discuss your project ideas and connect with the Nexus team. For potential funding and partnership opportunities, contact [growth@nexus.xyz](mailto:growth@nexus.xyz).

## How to Add Your Project

To add your project to this list:

1. Fork this repository
2. Add your project under the appropriate category
3. Submit a pull request with a clear description

All submissions will be reviewed by maintainers. See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

