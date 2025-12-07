# MyToken (MTK) - ERC-20 Token Smart Contract

## Overview
MyToken is a simple, beginner-friendly ERC-20 compatible token built on Ethereum for learning blockchain development fundamentals. This implementation demonstrates core concepts of token standards, smart contracts, and decentralized finance.

## Token Details
- **Name**: MyToken
- **Symbol**: MTK
- **Decimals**: 18 (standard Ethereum precision)
- **Total Supply**: Configurable at deployment
- **Standard**: ERC-20 compliant
- **Solidity Version**: ^0.8.0

## Features
- ✅ Full ERC-20 standard implementation
- ✅ Transfer tokens between addresses
- ✅ Approve and transferFrom for delegated spending
- ✅ Balance tracking for all addresses
- ✅ Event emission for transparency (Transfer, Approval)
- ✅ Built-in safety with Solidity 0.8.x overflow protection
- ✅ Zero address validation
- ✅ Comprehensive error messages
- ✅ Helper functions for easy interaction

## Smart Contract Functions

### Core ERC-20 Functions

#### `balanceOf(address owner) → uint256`
Returns the token balance of the specified address.

**Example:**
```solidity
balanceOf(0x123...) // Returns: 1000000000000000000000 (1000 tokens with 18 decimals)
```

#### `transfer(address to, uint256 value) → bool`
Transfers tokens from the caller's address to another address.

**Parameters:**
- `to`: Recipient address
- `value`: Amount of tokens to transfer (in smallest units)

**Validations:**
- Recipient cannot be zero address
- Sender must have sufficient balance

**Example:**
```solidity
transfer(0x456..., 1000000000000000000) // Transfers 1 MTK
```

#### `approve(address spender, uint256 value) → bool`
Allows another address to spend tokens on your behalf.

**Parameters:**
- `spender`: Address authorized to spend
- `value`: Maximum amount they can spend

**Validations:**
- Spender cannot be zero address

**Example:**
```solidity
approve(0x789..., 500000000000000000) // Approves 0.5 MTK
```

#### `transferFrom(address from, address to, uint256 value) → bool`
Transfers tokens on behalf of another address (requires prior approval).

**Parameters:**
- `from`: Token owner address
- `to`: Recipient address
- `value`: Amount to transfer


MyToken.sol - A production-ready ERC-20 token contract featuring:

Full standard compliance with all required functions
Token metadata (MyToken/MTK, 18 decimals)
Complete transfer, approve, and transferFrom functionality
Comprehensive validation (zero address, balance, allowance checks)
Event emission for transparency
Helper functions for easy interaction
Clean, beginner-friendly comments
README.md - Extensive documentation covering:

Complete deployment guide for RemixIDE
Detailed function documentation with examples
Step-by-step testing instructions
Decimal handling explanation
Testnet deployment guide
Troubleshooting section
Security considerations and best practices
FAQ and additional resources
Quick Start
Open https://remix.ethereum.org/
Create a new file named MyToken.sol
Copy the contract code from your project
Compile with Solidity 0.8.x
Deploy with initial supply (e.g., 1000000000000000000000000 for 1M tokens)
Start testing transfers, approvals, and allowances
the token is now ready to deploy and test. The README provides comprehensive guidance for every step from compilation to advanced testing scenarios.
W2B
