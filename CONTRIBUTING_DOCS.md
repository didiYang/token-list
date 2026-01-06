# PancakeSwap Token List Contribution Documentation

This document provides additional guidance for contributors looking to understand the structure and maintenance of the PancakeSwap token lists, especially in the context of its Uniswap V2 heritage on the BNB Chain.

## Repository Overview

PancakeSwap is a prominent fork of Uniswap V2 deployed on the BNB Smart Chain (BSC). This repository manages the token lists used by the PancakeSwap interface.

### Key Directories

- `src/tokens`: Contains the raw token data in JSON format.
- `lists/`: Contains the generated token lists that are served to the frontend.
- `test/`: Contains validation tests to ensure token lists meet the required schema.

## BNB Chain Specifics

When adding tokens for the BNB Chain:
1. Ensure the `chainId` is set to `56` for BNB Smart Chain Mainnet.
2. Verify that the token address is the correct BEP-20 address on BSC.
3. Logos should be hosted on a reliable CDN or included in the `lists/images` directory if applicable.

## Uniswap V2 Compatibility

As a Uniswap V2 fork, PancakeSwap follows the [Token Lists](https://github.com/Uniswap/token-lists) specification. Any tool compatible with Uniswap token lists should be able to consume the JSON files generated in the `lists/` directory.

---
*Note: This documentation was added as part of a GitHub connector test.*
