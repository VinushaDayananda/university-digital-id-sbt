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
  ___ README.md
  ___.gitignore
  ___LICENSE
  ___docs/
        ___architecture.md
        ___api_design.md
        ___smart_contract_design.md
        ___project_pruposal.pdf
        ___presentation.pdf

  ___frontend/
        ___index.html
        ___css/
              ___styles.css
        ___js/
              ___wallet.js
              ___student_dashboard.js
              ___admin_dashboard.js
              ___qr_generation.js
              ___api.js
        ___pages/
              ___student_dashboard.html
              ___request_token.html
              ___verify_identity.html
              ___admin_dashboard.html
              ___wallet_recovery.html
        ___assets/
              ___images/
              ___icons/

  ___backend/
        ___app.py
        ___config.py
        ___requirements.txt
        ___databse/
              ___db.py
              ___scheme.sql
        ___models/
              ___student_model.py
              ___token_model.py
              ___request_model.py
              ___wallet_change_model.py
        ___routes/
              ___token_routes.py
              ___verification_routes.py
              ___admin_routes.py
              ___student_routes.py
        ___services/
              ___blockchain_service.py
              ___qr_service.py
        ___utils/
              ___helper.py
              ___validation.py

  ___blockchain/
        ___contracts/
              ___studentIdentitySBT.sol
        ___scripts/
              ___deploy.js
              ___intercat.js
        ___test/
              ___contract_test.js
        ___hardhat.config.js
        ___package.json
  ___diagrams/
        ___system_architecture.png
        ___data_flow.png
        ___smart_contract_flow.png


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
