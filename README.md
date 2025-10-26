# 🏥 MedCard NFT - Decentralized Medical Records Platform

> **Secure, Private, and Patient-Owned Healthcare Data on Blockchain**

[![Solidity](https://img.shields.io/badge/Solidity-^0.8.30-363636?style=for-the-badge&logo=solidity)](https://soliditylang.org/)
[![OpenZeppelin](https://img.shields.io/badge/OpenZeppelin-5.0-4E5EE4?style=for-the-badge&logo=openzeppelin)](https://www.openzeppelin.com/)
[![Foundry](https://img.shields.io/badge/Foundry-Latest-orange?style=for-the-badge)](https://book.getfoundry.sh/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Architecture](#-architecture)
- [Revenue Model & Financial Projections](#-revenue-model--financial-projections)
- [Technology Stack](#-technology-stack)
- [Installation](#-installation)
- [Usage](#-usage)
- [Security](#-security)
- [Video Demonstration Guide](#-video-demonstration-guide)
- [Roadmap](#-roadmap)

---

## 🎯 Project Overview

**MedCard NFT** is an innovative Web3 platform for managing medical records on blockchain. The project solves a critical problem in modern healthcare: patients lack complete control over their medical data.

### The Problem
- 🔒 **Centralized storage** — data is held by hospitals/clinics
- 🚫 **No patient control** — unable to manage access permissions
- 📄 **Paper-based records** — loss, damage, forgery risks
- 🌐 **System incompatibility** — clinics don't share data seamlessly

### Our Solution
```
┌─────────────────────────────────────────────────────────┐
│  PATIENT (NFT Owner)                                    │
│  ✅ Full control over medical data                      │
│  ✅ Manage doctor access permissions                    │
│  ✅ Portable medical records                            │
│  ✅ Transparent change history                          │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  BLOCKCHAIN (Smart Contract)                            │
│  • Stores metadata & access control                     │
│  • Permission management (grant/revoke)                 │
│  • Immutable audit trail                                │
└─────────────────────────────────────────────────────────┘
                          ↓
┌─────────────────────────────────────────────────────────┐
│  IPFS/Pinata (Encrypted Data)                           │
│  • Medical records (diagnosis, tests)                   │
│  • Medical imaging (X-rays, MRI)                        │
│  • Treatment history                                    │
└─────────────────────────────────────────────────────────┘
```

---

## 🚀 Key Features

### For Patients
- **👤 Complete Data Ownership** — NFT = property rights over medical card
- **🔐 Privacy First** — encrypted data stored off-chain
- **⚡ Instant Access** — doctors receive history in seconds (with permission)
- **🌍 Global Portability** — medical card accessible worldwide

### For Doctors
- **📊 Complete Patient History** — all data in one place
- **🔒 Legal Access** — only with explicit patient permission
- **💼 Risk Reduction** — transparent treatment history
- **⏱️ Time Savings** — no paperwork, instant data retrieval

### For Healthcare Institutions
- **💰 Monetization** — integration fees & commissions
- **📉 Cost Reduction** — less paperwork and administrative overhead
- **⚖️ GDPR Compliance** — patients control their own data
- **🔗 Interoperability** — standardized data exchange

---

## 💰 Revenue Model & Financial Projections

### Pricing Structure

| Service | Price | Revenue Share |
|---------|-------|---------------|
| NFT Minting | **0.01 ETH** | 100% Platform |
| Access Subscription (Doctor) | $10/month | Recurring Revenue |
| Premium Features | $5-25/month | Patient/Doctor tiers |
| API Integration (Clinics) | $500-5000/month | B2B Revenue |

### 3-Month Financial Projection

**Assumptions:**
- 500 new users/month
- Average ETH price: $2,500
- Mint price: 0.01 ETH = $25
- 30% doctor subscription conversion rate
- 10% premium user adoption

#### Monthly Breakdown

| Month | New Users | Total Users | NFT Mints | Mint Revenue (ETH) | Mint Revenue (USD) | Subscription Revenue | Total Monthly Revenue |
|-------|-----------|-------------|-----------|-------------------|-------------------|---------------------|----------------------|
| **Month 1** | 500 | 500 | 500 | 5 ETH | $12,500 | $1,500 | **$14,000** |
| **Month 2** | 500 | 1,000 | 500 | 5 ETH | $12,500 | $3,000 | **$15,500** |
| **Month 3** | 500 | 1,500 | 500 | 5 ETH | $12,500 | $4,500 | **$17,000** |

**3-Month Total Revenue: $46,500**

### 12-Month Growth Projection

```
📈 YEAR 1 PROJECTIONS (Conservative Scenario)

Users Growth:
Month 1-3:   500 users/month  → 1,500 total
Month 4-6:   750 users/month  → 3,750 total
Month 7-9:   1,000 users/month → 6,750 total
Month 10-12: 1,500 users/month → 11,250 total users

Revenue Breakdown (Year 1):
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
💎 NFT Minting:           $281,250  (11,250 mints × $25)
🔄 Subscriptions:         $168,750  (recurring monthly)
⭐ Premium Features:      $42,000   (10% adoption)
🏥 B2B Integrations:      $60,000   (10 clinics × $500/month)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
💰 TOTAL YEAR 1 REVENUE:  $552,000
```

### Key Performance Indicators (KPIs)

| Metric | Month 1 | Month 3 | Month 12 | Target Year 2 |
|--------|---------|---------|----------|---------------|
| **Active Users** | 500 | 1,500 | 11,250 | 50,000 |
| **Total NFTs Minted** | 500 | 1,500 | 11,250 | 50,000 |
| **Doctor Subscribers** | 150 | 450 | 3,375 | 15,000 |
| **Monthly Revenue** | $14K | $17K | $65K | $300K |
| **Clinic Integrations** | 2 | 5 | 10 | 50 |

### Cost Structure (Monthly)

| Expense Category | Month 1-3 | Month 6-12 |
|------------------|-----------|------------|
| Infrastructure (AWS, IPFS) | $500 | $2,000 |
| Smart Contract Gas Fees | $300 | $1,000 |
| Development Team | $8,000 | $15,000 |
| Marketing & Growth | $2,000 | $8,000 |
| Legal & Compliance | $1,000 | $2,000 |
| **Total Monthly Costs** | **$11,800** | **$28,000** |

**Net Profit Margin:**
- Months 1-3: ~18% ($2,200/month average)
- Months 6-12: ~40% ($17,000/month average)
- Year 1 Total: ~35% net margin

---

## 🏗 Architecture

### Smart Contract Structure

```solidity
contract MedicalCardNFT is ERC721Enumerable, ERC721URIStorage, Ownable {
    
    // ═══════════════════════════════════════════════════════
    //  CORE FUNCTIONS
    // ═══════════════════════════════════════════════════════
    
    /// @notice Mint new medical card NFT (0.01 ETH)
    function safeMint(
        address to, 
        string tokenMetadataUri,  // Public IPFS metadata
        string initialPrivateUri  // Encrypted medical data CID
    ) payable returns (uint256)
    
    /// @notice Grant doctor access to medical records
    function grantAccess(uint256 tokenId, address doctor)
    
    /// @notice Revoke doctor access
    function revokeAccess(uint256 tokenId, address doctor)
    
    /// @notice Check if address has access
    function hasAccess(uint256 tokenId, address addr) returns (bool)
    
    /// @notice Get private medical data URI (encrypted)
    function getPrivateTokenURI(uint256 tokenId) returns (string)
    
    /// @notice Update medical records (owner or authorized doctor)
    function updatePrivateData(uint256 tokenId, string newPrivateUri)
}
```

### Data Flow

```
1. MINTING FLOW:
   Patient → Frontend → Smart Contract (0.01 ETH) → NFT Created
                              ↓
                     IPFS Upload (Encrypted Medical Data)
                              ↓
                     Private CID stored in contract

2. ACCESS CONTROL FLOW:
   Patient grants access → Smart Contract records permission
                              ↓
   Doctor requests data → Contract verifies permission
                              ↓
   Frontend fetches IPFS → Decrypts with patient's key
                              ↓
   Doctor views medical records

3. UPDATE FLOW:
   Doctor/Patient → Upload new data to IPFS
                              ↓
                     Update private CID in contract
                              ↓
                     Emit event for audit trail
```

### Security Model

| Layer | Security Measure |
|-------|------------------|
| **Smart Contract** | OpenZeppelin audited contracts, Access control modifiers |
| **Data Encryption** | AES-256 encryption before IPFS upload |
| **Access Control** | On-chain permission registry, Time-limited access tokens |
| **Key Management** | Patient-controlled encryption keys, Optional multi-sig |
| **Audit Trail** | All operations emit events, Immutable blockchain history |

---

## 🛠 Technology Stack

### Blockchain & Smart Contracts
- **Solidity** ^0.8.30 — Smart contract language
- **OpenZeppelin** 5.0 — Battle-tested contract libraries
- **Foundry** — Development framework & testing
- **Ethers.js** 5.7.2 — Blockchain interaction library

### Storage & Infrastructure
- **IPFS** — Decentralized file storage
- **Pinata** — IPFS pinning service (enterprise-grade)
- **Encryption** — Client-side AES-256-GCM

### Frontend
- **HTML5/CSS3/JavaScript** — Pure vanilla JS (no framework dependencies)
- **Web3 Provider** — MetaMask integration
- **Responsive Design** — Mobile-first approach

### Supported Networks
- ✅ Ethereum Mainnet
- ✅ Polygon (low gas fees)
- ✅ Xsolla ZK Sepolia (testnet)
- ✅ Arbitrum / Optimism (L2 solutions)

---

## 📦 Installation

### Prerequisites

```bash
# Required software versions
Node.js: >= 18.0.0
Foundry: latest
MetaMask: browser extension
Git: >= 2.30.0
```

### Step 1: Clone Repository

```bash
git clone https://github.com/ZeroNewLife/finalProject.git
cd finalProject
```

### Step 2: Install Dependencies

```bash
# Install Foundry dependencies
forge install

# Install frontend dependencies
cd frontend
npm install
cd ..
```

### Step 3: Configure Environment

Create `.env` file in root directory:

```env
# Wallet Configuration
PRIVATE_KEY=your_wallet_private_key_here

# Network Configuration
RPC_URL=https://eth-sepolia.g.alchemy.com/v2/YOUR_API_KEY
SEPOLIA_RPC_URL=https://rpc.ankr.com/eth_sepolia

# IPFS Configuration (Optional)
IPFS_GATEWAY=https://gateway.pinata.cloud
PINATA_API_KEY=your_pinata_api_key
PINATA_API_SECRET=your_pinata_secret

# Contract Configuration
MINT_PRICE=0.01
```

⚠️ **Security Warning:** Never commit `.env` file to Git. Add it to `.gitignore`.

### Step 4: Deploy Smart Contract

```bash
# Deploy to Xsolla ZK Sepolia testnet
forge script script/Deploy.s.sol \
  --rpc-url $SEPOLIA_RPC_URL \
  --private-key $PRIVATE_KEY \
  --broadcast \
  --verify

# Save the deployed contract address
# Example output: NFT deployed to: 0xA05A6361339f018712E292b32362cf8a2c610F5f
```

### Step 5: Configure Frontend

Edit `frontend/index.html`, update line ~420:

```javascript
const CONFIG = {
    CONTRACT_ADDRESS: '0xYOUR_DEPLOYED_CONTRACT_ADDRESS',
    MINT_PRICE: '0.01',
    // ... rest of config
};
```

### Step 6: Run Application

```bash
cd frontend
npm run start
# or
python3 -m http.server 8000

# Open browser: http://localhost:8000
```

---

## 📖 Usage

### For Patients

#### 1. Connect Wallet
```javascript
// Click "Connect MetaMask" button
// Approve connection in MetaMask popup
// Your wallet address will be displayed
```

#### 2. Create Medical Card NFT
```javascript
// Fill in the form:
- Full Name: "John Doe"
- Date of Birth: "1990-01-15"
- Diagnosis: "Type 2 Diabetes"
- Additional Info: "Allergic to penicillin"

// Click "Create Medical Card NFT"
// Approve 0.01 ETH transaction in MetaMask
// Wait for confirmation (~15 seconds)

// Result: NFT minted, medical data encrypted & stored on IPFS
```

#### 3. Manage Doctor Access
```javascript
// Load your NFTs
// Click "Manage Access" on a card
// Enter doctor's wallet address: 0x742d35Cc6634C0532925a3b844Bc9e7595f0bEb
// Click "Grant Access"
// Approve transaction

// To revoke: same process, click "Revoke Access"
```

### For Doctors

#### 1. Request Access
```markdown
1. Patient provides their NFT Token ID
2. Patient grants your wallet address access via frontend
3. You receive notification (off-chain via email/app)
```

#### 2. View Medical Records
```javascript
// Connect your wallet (as doctor)
// Enter patient's Token ID
// Click "View Private Data"
// System verifies your on-chain permission
// Encrypted data fetched from IPFS & decrypted
// View full medical history
```

#### 3. Update Records (if permitted)
```javascript
// Navigate to patient's medical card
// Click "Update Medical Data"
// Upload new test results, diagnosis, prescriptions
// Data encrypted & new IPFS CID stored on-chain
// Patient receives update notification
```

### API Usage (For Clinic Integration)

```javascript
// Example: Programmatic minting
const ethers = require('ethers');

const provider = new ethers.providers.JsonRpcProvider(RPC_URL);
const wallet = new ethers.Wallet(PRIVATE_KEY, provider);
const contract = new ethers.Contract(CONTRACT_ADDRESS, ABI, wallet);

async function mintForPatient(patientAddress, medicalDataCID) {
    const tx = await contract.safeMint(
        patientAddress,
        `ipfs://${publicMetadataCID}`,
        `ipfs://${medicalDataCID}`,
        { value: ethers.utils.parseEther("0.01") }
    );
    
    const receipt = await tx.wait();
    console.log(`NFT minted! Token ID: ${receipt.events[0].args.tokenId}`);
    return receipt;
}
```

---

## 🔒 Security

### Smart Contract Security

✅ **Audited Libraries** — OpenZeppelin contracts (industry standard)  
✅ **Access Control** — Ownable, role-based permissions  
✅ **Reentrancy Protection** — No external calls in state-changing functions  
✅ **Integer Overflow** — Solidity 0.8+ built-in protection  
✅ **Input Validation** — All parameters checked

### Data Privacy

| Security Feature | Implementation |
|------------------|----------------|
| **Encryption** | AES-256-GCM client-side encryption |
| **Key Storage** | Patient-controlled, never stored on-chain |
| **Access Control** | Blockchain-enforced permissions |
| **Data Location** | Off-chain IPFS, only encrypted CIDs on-chain |
| **Anonymity** | Wallet addresses, no personal identifiers on-chain |

### Best Practices

```markdown
🔐 SECURITY CHECKLIST FOR USERS:

✅ Never share your private key
✅ Use hardware wallet (Ledger/Trezor) for production
✅ Verify contract address before transactions
✅ Enable 2FA on MetaMask if available
✅ Regularly revoke unused doctor access permissions
✅ Backup encryption keys in secure location (password manager)
✅ Use strong passwords for IPFS pinning services
✅ Monitor on-chain events for unauthorized access attempts
```

### Known Limitations

⚠️ **Current Version Limitations:**
- Encryption key management is manual (future: MPC wallets)
- No built-in key recovery (use social recovery in future)
- IPFS relies on pinning service uptime (future: multiple providers)
- Gas costs on Ethereum L1 can be high (use L2 solutions)

---

## 🎥 Video Demonstration Guide

### Recommended Video Structure (10-15 minutes)

#### 1. Introduction (2 minutes)
```markdown
📹 SCENE 1: Problem Statement
- Show current healthcare data problems
- Statistics: data breaches, access delays
- Patient testimonials (mock/stock footage)

🎯 Hook: "What if patients owned their medical records like NFTs?"
```

#### 2. Solution Overview (3 minutes)
```markdown
📹 SCENE 2: Platform Walkthrough
- Show animated architecture diagram
- Explain blockchain + IPFS combination
- Highlight key benefits (privacy, control, portability)

🎬 Screen Recording Tips:
- Use 1920x1080 resolution
- Enable smooth cursor movements
- Highlight clicks with visual effects (OBS Studio)
```

#### 3. Live Demo (8 minutes)
```markdown
📹 SCENE 3: Patient Flow
[0:00-2:00] Connecting MetaMask wallet
[2:00-4:00] Creating medical card NFT
  - Show form filling
  - Display transaction in MetaMask
  - Confirm successful mint
[4:00-6:00] Granting doctor access
  - Enter doctor address
  - Show on-chain transaction
  - Verify access in contract

📹 SCENE 4: Doctor Flow
[6:00-7:30] Doctor connecting wallet
[7:30-8:30] Viewing patient records
  - Show permission check
  - Display decrypted medical data
  - Demonstrate update capability

🎬 Recording Tools:
- Screen: OBS Studio / Loom / ScreenFlow
- Audio: Blue Yeti microphone (clear narration)
- Editing: DaVinci Resolve (free) / Adobe Premiere
```

#### 4. Technical Deep Dive (2 minutes)
```markdown
📹 SCENE 5: Code Walkthrough
- Show smart contract code (key functions)
- Explain safeMint() with payment
- Show access control logic
- Display event logs in Etherscan

🎬 Code Display:
- Use VS Code with theme: "Dracula Official"
- Font: Fira Code (ligatures enabled)
- Zoom to 150% for readability
```

#### 5. Business Model (1 minute)
```markdown
📹 SCENE 6: Revenue & Growth
- Show financial projections table
- Animated graph of 12-month revenue
- Display user adoption curve
- End with call-to-action

🎬 Graphics:
- Use Canva Pro for infographics
- Chart.js for animated graphs
- Fade transitions between scenes
```

### Video Production Checklist

```markdown
PRE-PRODUCTION:
□ Write detailed script with timestamps
□ Prepare demo environment (testnet with test ETH)
□ Create 3-5 demo accounts (patient, doctors)
□ Pre-mint sample NFTs for demo
□ Design intro/outro graphics (project logo, links)

PRODUCTION:
□ Record in 4K (downscale to 1080p for quality)
□ Use second monitor for notes/script
□ Record audio separately (48kHz, 24-bit)
□ Multiple takes for each scene (pick best)
□ Capture B-roll: code, blockchain explorer, IPFS

POST-PRODUCTION:
□ Color correction (consistent brightness)
□ Audio leveling (-14 LUFS for YouTube)
□ Add background music (royalty-free)
□ Insert captions/subtitles (accessibility)
□ Add chapter markers in timeline
□ Export: H.264, 1080p, 60fps, 12Mbps bitrate

PUBLISHING:
□ YouTube SEO: title, description, tags
□ Create thumbnail (1280x720, faces + text)
□ Add timestamps in description
□ Include GitHub link, contract address
□ Pin comment with setup guide
```

### Sample Video Script

```markdown
[INTRO - 0:00]
"Healthcare data is broken. Patients don't control their records.
Hospitals hoard information. Data breaches expose millions.

What if there was a better way?

Welcome to MedCard NFT - where patients own their medical records
as blockchain NFTs, stored securely on IPFS, with granular access
control. Let me show you how it works."

[DEMO START - 0:30]
"I'm connecting my MetaMask wallet to the platform..."
[Continue with step-by-step narration]

[OUTRO - 14:30]
"MedCard NFT represents the future of healthcare data:
decentralized, private, and patient-owned.

Join us in revolutionizing medical records.
Contract address and GitHub link in the description.

Thanks for watching!"
```

---

## 🗺 Roadmap

### Phase 1: MVP (Current) ✅
- [x] Smart contract development
- [x] Basic frontend interface
- [x] IPFS integration
- [x] MetaMask connection
- [x] NFT minting with payment
- [x] Access control (grant/revoke)

### Phase 2: Q1 2026 🚧
- [ ] Mobile app (React Native)
- [ ] Advanced encryption (MPC wallets)
- [ ] Multi-signature recovery
- [ ] Doctor verification system (KYC)
- [ ] Notification system (email/push)
- [ ] Analytics dashboard

### Phase 3: Q2 2026 📋
- [ ] EHR system integrations (HL7 FHIR)
- [ ] Insurance company API
- [ ] Telemedicine integration
- [ ] Multi-chain deployment (Polygon, Arbitrum)
- [ ] Gasless transactions (meta-transactions)
- [ ] DAO governance

### Phase 4: Q3-Q4 2026 🌐
- [ ] AI-powered health insights
- [ ] Wearable device integration (Fitbit, Apple Watch)
- [ ] Research data marketplace (anonymized)
- [ ] International expansion (regulatory compliance)
- [ ] Enterprise white-label solution

---

## 🤝 Contributing

We welcome contributions! Please follow these guidelines:

1. Fork the repository
2. Create feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open Pull Request

**Code Style:**
- Solidity: Follow [Solidity Style Guide](https://docs.soliditylang.org/en/latest/style-guide.html)
- JavaScript: ESLint configuration provided
- Comments: Required for all public functions

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👥 Team

- **ZeroWeb3** - Smart Contract Development & Architecture
- **Doni** - Full-Stack Development & Frontend

---

## 📞 Contact & Support

- **GitHub Issues:** [Report bugs or request features](https://github.com/ZeroNewLife/finalProject/issues)
- **Email:** support@medcardnft.io
- **Twitter:** [@Zero](https://x.com/ZeroNewLif)
- **Discord:** [Join community](https://discord.gg/medcardnft)

---

## 🙏 Acknowledgments

- OpenZeppelin for secure smart contract libraries
- Foundry team for excellent development tools
- Pinata for reliable IPFS infrastructure
- Ethereum community for Web3 standards

---

<div align="center">

**⭐ Star this repository if you find it useful!**

Made with ❤️ by the MedCard NFT Team

[🌐 Website](https://medcardnft.io) • [📚 Docs](https://docs.medcardnft.io) • [🎥 Demo Video](https://youtube.com/medcardnft)

</div>
