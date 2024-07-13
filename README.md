# Individuum

Individuum is an onchain matching protocol for offchain intents. During this hackaton we built a marketplace for people to exchange twitter visibility. The buyer creates an order for a matching string in a tweet with a certain price per like (USDC) and a max budget allocation. Then some X user can prove using TLSNotary that he owns an account which has tweeted the required string and has an amount of likes. This proof is sent onchain where the contract built with arbitrum stylus pays the user for the amount of likes he got.

## Tech stack

<img width="1424" alt="Screenshot 2024-07-13 at 20 17 14" src="https://github.com/user-attachments/assets/cb444ea4-4f95-4fec-82eb-2883365f6763">

### Tracks
- TLSNotary
- Arbitrum Stylus
- USDC
- Web3Auth

### Repositories

- core: Arbitrum stylus smart contracts (Verifier, Escrow) built with Rust
- ui: Next.js web application using Web3Auth for user authentification
- plugin: Plugin for the TLSNotary chrome extension
- verifier: Trusted off-chain verifier built with Rust and the Axum web framework
