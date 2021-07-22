# Aletheia

Description
The project is currently at its infancy, but it's 3 distinct things:
- A feed agent that scrapes online prices to gauge the inflation of a particular national economy
- A decentralized Oracle that is based on the aforementioned agents to present the values inside the Ethereum blockchain, in a decentralized and crypto-economically secure manner
- a DeFi platform that uses inflation, as a data-point, to offer financial products (e.g inflation-adjusted vaults, etc.)

Currently, the agent feed is perfectly defined and ready to be developed, the decentralized oracle needs some refinement around its mechanism design (MEV implications, etc.) and the DeFi platform is completely undefined.

Aletheia - Inflation Oracle showcase

How it's made
The feed agent is coded in rust. It's a modular design that:
- Reads the scraping targets + inflation computation taxonomy from a pre-determined target
- Scrapes the URLs daily and computes the daily inflation index
- Computes a proof for the aforementioned computation
- Stores the raw data in a retrievable manner
- Outputs a package with the aforementioned data structures

The decentralized oracle is a set of smart contracts that organizes the feeds. The mechanism design needs refinement.



<p align="center">
  <img width="460" height="460" src="https://user-images.githubusercontent.com/13405632/124463274-558e7180-dd9b-11eb-8b9d-0aa2f0b7f851.png">
</p>

Aletheia (Or Alathea) was the spirit of truth, truthfulness, and sincerity. She had three opposites; Dolos, the god of trickery, Apate, the goddess of deception, and all the Pseudologoi, the gods of lies. Her Roman name was Veritas. She is either a daughter of Zeus or she was created by Prometheus.

Aletheia is the first decentralized inflation oracle


## Roadmap

- whitepaper: TBD
- version: `paper-napkin`

### MVP Inflation Feed
- [ ] aletheia -- orchestrator module
- [ ] hermes -- scraping module
- [ ] hephaestus -- computation module
- [ ] zephyrus -- p2p module (for [bitclout](https://bitclout.com))
- [ ] lethe -- archive module
- [ ] aether -- Ethereum blockchain interface module
- [ ] eunomia -- identity module

### Decentralized Oracle
TBD
### Inflation-Adjusted DeFi
TBD
