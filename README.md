---
description: 'Off-chain composability: our vision for a Web3 far beyond blockchains'
---

# Web3 beyond blockchains

## 1/4 - Web3 is trapped on-chain

Web3 looks like it's heading into a bright future. By combining incentives and cryptography, blockchains have achieved unprecedented decentralization and security, and general-purpose L1s like Ethereum now host growing ecosystems of interoperable decentralized protocols. There's everything from DeFi staples like the Compound lending platform to fascinatingly novel experiments like the cryptography game Dark Forest. Key technical problems like execution scalability now have breakthrough solutions like rollups and zero-knowledge proofs. And even the UX is steadily improving, allowing more and more regular users to join the "crypto" world.

But on a closer look, there's a big problem: **web3's revolution is trapped inside blockchains**. Smart contracts running on blockchains may have the strong neutrality, decentralization, and censorship-resistance that Web3 promises, but everywhere else, Web2's problems seem to crop up with a vengeance.

### Web3 gateways



Nowhere is this clearer than in "dApp frontends": off-chain programs used to interact with on-chain systems by inherently off-chain humans and devices. The typical dApp frontend is nakedly a Web2 service, with a centralized server hosting a webpage (like [app.uniswap.org](https://app.u)) calling a centralized SaaS service to interact with on-chain smart contracts on the user's behalf.&#x20;

<figure><img src="https://lh6.googleusercontent.com/5hjXD0MECAaWMoCLmJtvB2F_K0RfC4lhbdnZdTL44c7MROXfLVF45yngnX6F46UmZKfgLTSL971M4gcVMDbc0zBIVXe_z2q5xkiTeMnHpzCsPP2dwR4XrqCIzPUtLDhWUPenVhi-65S2WqErjE1ee0T1wQ=s2048" alt=""><figcaption></figcaption></figure>

Unsurprisingly, users are at the mercy of the same sort of unaccountable centralized power we see in Web2 — just witness how a single regulatory agency (OFAC) easily cut off access to a widely-used protocol (Tornado Cash) simply by putting pressure on a few service providers (Infura, etc).



<div>

<figure><img src="https://lh5.googleusercontent.com/AyrH9O5DkK7yizDIlXTbrqvSEf-ioRjJtEEuyB0yYdFyszrK9wn-JJIDyRdYkpUb-AlxcDCfmnU0oTE1vrpD03qwKImnZfGKic7dOuch1gTcLkZR7PSK2B6N0KdM2QsGEQpqYwEkRVGPIbHItNyGstaHNg=s2048" alt=""><figcaption><p>Tornado Cash</p></figcaption></figure>

 

<figure><img src=".gitbook/assets/pasted image 0.png" alt=""><figcaption><p>Wormhole</p></figcaption></figure>

 

<figure><img src=".gitbook/assets/pasted image 0 (1) (1).png" alt=""><figcaption><p>Merit Circle</p></figcaption></figure>

</div>



All of the smart contracts involved in Tornado Cash, Wormhole, and Merit Circle ran safely and correctly. But the apps—which include inherently off-chain frontends, infrastructure, etc—did not.

### Non-blockchain Web3

Moreover, there's a whole world of entirely non-blockchain projects that are arguably Web3 protocols — "alt-tech" protocols sharing the same goal of fixing Web2's problems with decentralized cryptography: Tor, Freenet, Matrix, and the like.&#x20;

Compared to blockchain apps, nearly all struggle to gain adoption due to the difficulty of successfully combining decentralization, usability, and security, a need that blockchains seem ideally suited to satisfy. Yet puzzlingly, we don't see much blockchain adoption in these projects that truly need decentralized security.

## 2/4 - Mel frees web3

We believe that the solution to this problem is a new paradigm for "Web3": **off-chain composability**. Instead of a complex on-chain ecosystem of smart contracts with "frontends" that struggle to interface with them, this will be a largely non-blockchain world with two key properties:

**Off-chain programs trustlessly compose with on-chain programs.** Off-chain programs, whether dApp frontends or whole alt-tech stacks, must integrate on-chain functionality without sacrificing L1 security.&#x20;

For instance, a frontend for a coin mixer can't be censorable by any SaaS provider, and no platform provider should be able to tamper with queries to an on-chain PKI used by an end-to-end encrypted chat program. The "web3 superpowers" end up successfully crossing over the boundaries of the blockchain.

**Decentralized protocols compose into dApps off-chain.** Decentralized protocols with blockchain-backed security should not primarily compose using on-chain constructs such as standardized smart-contract interfaces. Instead, they are composed in off-chain programs like mobile apps and frontends to create a "full-stack" decentralized system.&#x20;

For example, clients for a decentralized encrypted chat platform with cryptocurrency payments can be built from a Sybil-resistant DHT, a blockchain-backed naming system, a micropayment network, etc, all of which are protocols trustlessly compose with on-chain logic to provide robust decentralized security. But none of these systems need to have interoperating on-chain logic.&#x20;

_Explain how this solves all the issues_

## 3/4 - Why do we need another blockchain?

Mel is a new L1 blockchain designed completely from scratch. It focuses on one task: being the keystone of decentralized security that enables an off-chain composable Web3.

This affects every aspect of Mel's unique design, which we'll dive into in subsequent pages:

* The synergy between composability and neutrality in its data model: We use a stripped-down TXO-based model optimized for trustless off-chain queries that is intended to be simple enough to be _governance-free_ and thus robustly neutral. This turns out to both support and require a vibrant off-chain composable ecosystem.
* The consensus game: Mel's proof-of-stake consensus has two important features, both crucial to reliable off-chain thin-clients. First, it uses unique _collusion-resistant incentives_, ensuring long-run safety without external governance intervening. Second, it produces _long-range consensus proofs_ that minimizes "weak subjectivity" problems and allows for deeply embedded thin clients to stay economically secure.
* The mechanism, Melmint, behind the native currency MEL: Without any oracles or external trust, Melmint stabilizes MEL's value against the _cost of sequential computation time_, one of the few purchasing-power-stable indices that can be trustlessly defined and measured. This makes MEL as trustless as BTC and ETH, while still being a useful unit of account that avoids typical cryptocurrency price swings. It turns out that this is key to building off-chain composable financial systems.

&#x20;

## 4/4 - Up next: how Mel frees web3

##
