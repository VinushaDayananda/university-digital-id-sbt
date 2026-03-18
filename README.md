# university-digital-id-sbt
Blockchain-based University Digital Identity System using Soulbound Tokens

## Features
- Blockchain-based student identity
- One student = one SBT token
- Non-transferable identity tokens
- QR code verification system
- Student dashboard
- Admin dashboard
- Wallet revovery mechanism
- Secure identity verification

## System Architecture
The system consists of three main layers:

  01. Frontend Layer
      User interfaces for students and administrators

      Functions:
      - Student dashboard
      - Token request
      - Identity verification
      - QR code generation
      - Wallet connection

      Technologies:
      - HTML
      - CSS
      - JavaScript
      - Web3 wallet integration

02. Backend Layer
    Handles API logic, databse management and blockchain interaction.

    Functions:
    - Token issuance API
    - Token revocation API
    - Token verification API
    - Student management
    - QR code generation

    Technologies:
    - Python (FLask)
    - REST API
    - SQL Database

03. Blockchain Layer
    Implement the Soulbound Token smart contracts

    Functions:
    - Mint student identity token
    - Revoke token
    - Verify token
    - Ownership check
    - Transfer restriction (non-tranferable)
   
    Technologies:
    - Solidity
    - Hardhat
    - Etherium compatible network

