<h1 align="center"><b>Hi </b><img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="35"></h1>

Senior Backend Engineer. Go first, with six years of backend and blockchain infrastructure.

I build backend systems that stay correct under load, retries and partial failure.

**Backend.** Most of my work is the code that moves money and has to be exactly right. At Qiro, I designed
an append-only credit ledger with exact-money arithmetic and invariants enforced in PostgreSQL, so two
workers racing on the same event can't both commit, and event ingestion from two independent sources
with idempotent writes and automatic gap detection. Before that, I built a deadline-bounded auction in Go
that fans out to many upstreams and returns the best answer before a hard 12-second cutoff, and a
real-time matching engine on an in-memory order book with disk kept off the hot path and crash recovery
by replay.
I care about the parts that break in production: retries, races, partial failure, and backpressure.

**Infrastructure.** At Tokamak I led a team of four building a Go SDK and CLI that provisions cloud
infrastructure and deploys a full service stack to Kubernetes from one command. It's resumable when a
step fails halfway. I also own observability in Prometheus and Grafana and use it to diagnose live
incidents, not just to draw dashboards.

**Blockchain.** The same distributed-systems problems, on a chain. I've built reorg-safe EVM indexers,
off-chain matching with on-chain settlement, P2P networking on libp2p, and Solidity contracts for perps
and cross-chain protocols. I've also contributed to go-ethereum.

## Selected work

| Project | What it proves |
|---|---|
| [**payments-platform**](https://github.com/Shailu-s/payments-platform) | Money movement through unreliable providers on a double-entry, immutable ledger. Go, PostgreSQL, Kafka. In progress. |
| [**shortn**](https://github.com/Shailu-s/shortn) | URL shortener load-tested until it broke. 37,893 redirects/s, p95 2.32 ms, measured on one laptop, and the bugs that only showed up under load. |
| [**p2p-relayer**](https://github.com/Shailu-s/p2p-relayer) | Leader-follower P2P matching engine with an off-chain order book. 500+ orders/s sustained in production. |
| [**p2p-messenger**](https://github.com/Shailu-s/p2p-messenger) | Decentralized messenger on libp2p gossipsub. Store-and-forward for offline peers, and Double Ratchet encryption so one stolen key opens exactly one message. |
| [**Spool-EVM-indexer**](https://github.com/Shailu-s/Spool-EVM-indexer) | Config-driven event indexer for any EVM chain into PostgreSQL. Reorg-safe through confirmation depth and block-hash rollback. |
| [**trh-sdk**](https://github.com/tokamak-network/trh-sdk) | Go SDK and CLI that provisions and deploys a full rollup stack to Kubernetes from one command. I led the team of four that built it. |

## Tech Stack
**Languages**

![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Solidity](https://img.shields.io/badge/Solidity-363636?style=for-the-badge&logo=solidity&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

**Data & messaging**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/RabbitMQ-FF6600?style=for-the-badge&logo=rabbitmq&logoColor=white)
![gRPC](https://img.shields.io/badge/gRPC-244C5A?style=for-the-badge)

**Infrastructure & observability**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)

**Blockchain**

![Ethereum](https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=ethereum&logoColor=white)
![go-ethereum](https://img.shields.io/badge/go--ethereum-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![Foundry](https://img.shields.io/badge/Foundry-1C1C1C?style=for-the-badge)
![libp2p](https://img.shields.io/badge/libp2p-469EA2?style=for-the-badge)

---

[Portfolio](https://shailu-s.github.io) · [LinkedIn](https://www.linkedin.com/in/shailendrasinghw3/) · [X](https://x.com/0xshailu) · [Email](mailto:srajawat024@gmail.com)
