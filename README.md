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


