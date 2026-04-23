# X-Cash Migration results. Merkle Distribution

This repository contains the Merkle tree dataset used for XCash token distribution.

## Details

- Merkle root: 0xea08745d6dc6173f0333e1468423fa17bcbba4acc5045b1f9116f949ce061896
- Standard: Uniswap/OpenZeppelin-compatible Merkle distributor
- Leaf encoding: keccak256(abi.encodePacked(index, account, amount))
- Proof format: bytes32[]
- Hashing: keccak256 with sorted pairs
- Chain: <chain_id>
- Token: <token_address>

## Files

- `merkle_tree_<timestamp>.json` — full distribution dataset
- includes:
  - index
  - address
  - amount (wei)
  - proof

## Verification

Proofs can be verified using OpenZeppelin `MerkleProof.verify`.

## Source

- Source dataset SHA256: <hash>
- Generated at: <timestamp>
