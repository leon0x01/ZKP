### INTRODUCTION 

1. ZeroKnowledge is the ability to prove honest computation without revealing inputs
2. Zero-Knowledge proofs are cryptographic protocols that enable one party(the prover) to prove to another party(the verifier) that a particular statement is true without revealing any additional information about the statement beyond its validity.
3. The term "zero-knowledge" refers to the fact that the verifier learns nothing else about the statement or the underlying data apart from its truthfulness.

Example of [Zero Knowledge Proofs](!https://www.youtube.com/watch?v=5qzNe1hk0oY)

The Current ZKP systems that have been developed over the years are:

ZK-SNARKs (Zero-Knowledge Succinct Non-Interactive Argument of Knowledge): ZK-SNARKs are highly efficient non-interactive ZKPs that allow a prover to generate a proof that can be verified very quickly. They were popularized by the Zcash cryptocurrency and have since found applications in privacy-preserving smart contracts, blockchain scalability solutions, and more.

Bulletproofs: Bulletproofs are non-interactive zero-knowledge proofs that provide efficient range proofs for confidential transactions. They enable proving that a secret value lies within a specified range without revealing the exact value. Bulletproofs have been used in privacy-enhancing cryptocurrencies like Monero to improve scalability and reduce transaction sizes.

zk-STARKs (Zero-Knowledge Scalable Transparent ARguments of Knowledge): zk-STARKs are a type of zero-knowledge proof that provides transparency, scalability, and post-quantum security. They are designed to be highly efficient and allow for the verification of complex computations on large data sets. zk-STARKs have applications in blockchain, voting systems, and more.

zk-SNARKs and zk-STARKs derivatives: Various derivatives and improvements have been proposed for both zk-SNARKs and zk-STARKs, aiming to enhance efficiency, reduce trusted setup requirements, improve security, or address specific use cases. Examples include Sonic, Plonk, Marlin, Aurora, and Hyrax.

ZKPs based on cryptographic assumptions: Zero-knowledge proof systems can also be built based on specific cryptographic assumptions or hardness assumptions. For example, there are ZKP constructions based on the Discrete Logarithm Problem (DLP), the Quadratic Residue Problem (QRP), or lattice-based assumptions like Learning With Errors (LWE).


### What is a zk-SNARK?

zk-SNARKS(Zero-Knowledge Succinct Non-Interactive Arguments of KNOWLEDGE) is a cryptographic proof system that enables a prover to convince a verifier of the truth of a statement without revealing any additional information beyond the statement's validity. It involves a **setup phase** where public parameters are generated, a **proving phase** where the prover constructs a garbled arithmetic circuit and generates polynomial proofs based on a witness, and a **verification phase** where the verifier checks the validity of the proof using the public parameters, zk-SNARKS provide completeness, soundness, zero-knowledge and succinctness, making them valuable for privacy-preserving applications, blockchain systems, and more, although they rely on trusted setups and cryptographic assumptions.

#### zk-SNARK: Blockchain Applications

Scalability: SNARK Rollup(zk-SNARK for privacy from public)

    It utilizes zk-SNARKs to aggregate and validate multiple transactions off-chain while providing strong privacy guarantees by keeping the transaction details private from the public.

Privacy: Private Tx on a public Blockchain

    Confidential transactions
    Tornado cash
    Private Dapps: Aleo
    
Compliance:

    Proving Solvency in zero-knowledge
    Zero-knowledge taxes

### Protocols:

- Loopring
- Polygon Hermez
- ZKSync
- Zk Swap

#### Pros

- Smaller Proof size
- Smaller verification time
- Bigger developer community and libraries ( longer in the game)


#### Cons

- Required trusted setup (honest participants needed)
- Longer prover time
- Not secure by quantum computers
- Strong crypto assumptions
(The weaker the assumptions of a model, the stronger the model. Relaxing an assumption is to go from a strong to a weak, more realistic, assumption.)

### What is Zk-Stark?

Zk-Stark, which is stands for Zero-Knowledge Scalable Transparent Argument of Knowledge, is a cryptographic proof system that allows for the verification of computations without revealling any sensitive information about the computation itself. The key feature of ZK-STARKs is that they are transparent, which means the generation of the proof can be easily  verified by anyone without requiring any trusted setup or specialized knowledge. This transparency is desirable in various scenarios particularly in public blockchain networks where trust is distributed among multiple participants. Zk-STARKs are also post-quantum secure, meaning they are resistant to attacks by quantum computers. 

### Protocols:

- StarkWare/StarkEx
- Immutable X (StarkEx)
- DYDX (StarkEx)
- Starknet
- Polygon Miden

### Pros:

- Quantum Resistant
- Assumptions: Collision resistant hashes( less likely to be attacked)
- No Trusted Setup required
- Community Support by Ethereum Foundation
- More scalable in terms of computational speed


### Cons:

- Far Larger proof Size = More Gas
- Small Deverloper community becuase it is new