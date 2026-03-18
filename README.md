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

## Project Structure

university-digital-id-sbt/
│
├── README.md
├── .gitignore
├── LICENSE
│
├── docs/
│   ├── architecture.md
│   ├── api_design.md
│   ├── smart_contract_design.md
│
├── frontend/
│   ├── index.html
│   ├── css/
│   │   └── styles.css
│   │
│   ├── js/
│   │   ├── wallet.js
│   │   ├── student_dashboard.js
│   │   ├── admin_dashboard.js
│   │   ├── qr_generator.js
│   │   └── api.js
│   │
│   ├── pages/
│   │   ├── student_dashboard.html
│   │   ├── request_token.html
│   │   ├── verify_identity.html
│   │   ├── admin_dashboard.html
│   │   └── wallet_recovery.html
│   │
│   └── assets/
│       ├── images/
│       └── icons/
│
├── backend/
│   ├── app.py
│   ├── config.py
│   ├── requirements.txt
│   │
│   ├── database/
│   │   ├── db.py
│   │   └── schema.sql
│   │
│   ├── models/
│   │   ├── student_model.py
│   │   ├── token_model.py
│   │   ├── request_model.py
│   │   └── wallet_change_model.py
│   │
│   ├── routes/
│   │   ├── token_routes.py
│   │   ├── verification_routes.py
│   │   ├── admin_routes.py
│   │   └── student_routes.py
│   │
│   ├── services/
│   │   ├── blockchain_service.py
│   │   └── qr_service.py
│   │
│   └── utils/
│       ├── helpers.py
│       └── validators.py
│
├── blockchain/
│   ├── contracts/
│   │   └── StudentIdentitySBT.sol
│   │
│   ├── scripts/
│   │   ├── deploy.js
│   │   └── interact.js
│   │
│   ├── test/
│   │   └── contract_test.js
│   │
│   ├── hardhat.config.js
│   └── package.json
│
└── diagrams/
    ├── system_architecture.png
    ├── data_flow.png
    └── smart_contract_flow.png
    
##Steup Instructions
  01. Clone Repository
       git clone https://guthub.com/VinushaDayananda/university-digital-id-sbt.git
       cd university-digital-id-sbt

  02. Backend Setup
       cd backend
       pip install -r requirements.txt
       python app.py

  03. Blockchain Setup
       cd blockchain
       npm install
       npx hardhat compile
       npx hardhat run script/deploy.js

  04. Frontend
       open: frontend/index.html

##Diagrams
  system diagrams are available in:
      - System architecture
      - Data flow
      - Smart contract flow
##Future Improvements
       - Mobile wallet integration
       - Multi=university support
       - Decentralized storage (IPFS)
       - Zero-knowledge verification
       - Attendance,grading or payment systems
##License
       - MIT License
