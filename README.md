🛡️ Medical Card NFT: Secure & Profitable Decentralized Health Records

Abstract

This repository presents the smart contract and strategic roadmap for a decentralized medical card NFT system. The project prioritizes patient data privacy and ownership by storing sensitive medical records encrypted off-chain (IPFS/Pinata) while utilizing the NFT on-chain to manage strict access permissions (granting temporary access to doctors). The core goal is to generate scalable revenue through a standard minting fee.

💰 Financial Analysis & 3-Month Projection

The project's revenue engine is the 0.01 ETH minting fee paid by users. This forecast outlines a strong profitability model, driven by the low gas cost relative to the mint price.

Key Financial Assumptions & Metrics

Metric	Value	Notes
Mint Price (P)	0.01 ETH	Fixed price per NFT.
Current ETH Price	≈$3,500	Used for fiat conversion (Adjust as needed).
Revenue per Mint	≈$35.00	Gross revenue before gas.
Gas Cost (C)	≈$1.30	Average transaction gas cost (paid by the minter).
Net Revenue per Mint	≈$33.70	P−C.
Assumed Mints per Month (Q)	500 NFTs	Conservative adoption target for the initial phase.


3-Month Revenue Forecast

Assuming a conservative monthly growth, the project shows significant early potential:
Period	Mints (Q)	Gross ETH Revenue (ETH)	Net USD Revenue ($)	Cumulative Net USD ($)
Month 1	500	5.0 ETH	≈$16,850	≈$16,850
Month 2	600	6.0 ETH	≈$20,220	≈$37,070
Month 3	750	7.5 ETH	≈$25,275	≈$62,345


This forecast projects over $60,000 in net revenue, demonstrating the model's viability. The low operational cost (gas is only 3.7% of the mint fee) guarantees high profit margins.

🚀 Project Modernization & Growth Strategy

The long-term vision requires strategic scaling and integration to overcome Ethereum's gas constraints and achieve mass adoption.

1. Technical Optimization & L2 Migration

Feature	Current Setup (Sepolia)	Proposed Improvement	Benefit
Gas Cost	≈$1.30 per TX	L2 Migration (Polygon/Optimism)	Reduces transaction cost to $0.01 - $0.05, making it affordable for daily use.
Payment Stability	Volatile ETH Fee	Stablecoin Fees (USDC/DAI)	Provides predictable revenue and clear pricing for non-crypto users.
Data Integrity	Standard IPFS Link	Decentralized Storage + Proofs	Integrate with Filecoin/IPFS via services like Estuary and use ZK-proofs for data integrity assurance.
Access Control	Standard Ownable	Role-Based Access Control (RBAC)	Implement AccessControl for granular permissions (e.g., separate roles for Minter, Auditor, Data_Manager).


. Marketing & Ecosystem Development

    B2B Partnerships: Target Telemedicine platforms and Health Insurance providers to integrate the NFT as a standardized, tamper-proof Patient ID. This provides a clear, high-volume path to adoption.

    Web2 User Experience: The frontend must abstract away all blockchain complexity. Users should pay via fiat/Xsolla and interact with the NFT as a "digital pass," making the experience feel like a familiar SaaS product.

    Decentralized App (dApp) Ecosystem: Encourage external developers to build tools on top of the Medical Card standard (e.g., patient portals, medical billing services) using our public contract functions.

📚 Technical Overview & Workflow

Contract Architecture (src/MedicalCard.sol)

The contract is built on the robust foundation of OpenZeppelin libraries and customized logic to manage data separation:
Component	Key Feature
Data Separation	Stores public URI (tokenURI) and private encrypted URI (_privateTokenUris) separately.
Access Control	Uses _authorizedDoctors mapping for explicit permissions, enforced by the hasAccess function.
Trusted Minting	All token creation is restricted to the pre-set minterServiceAddress (your backend/Xsolla webhook).

Core Workflow: Data to NFT

Client Encryption: Patient data is encrypted off-chain (e.g., using their public key or an AES key).

IPFS Upload: The encrypted file is pinned to IPFS → generates ipfs://privateCid.

Metadata Prep: Public metadata JSON (linking to baseImageURI) is prepared → generates ipfs://metadataCid.

Minting: The Xsolla Webhook calls the contract:

safeMint(patientAddress, "ipfs://metadataCid", "ipfs://privateCid")

Access: The Patient grants access: grantAccess(tokenId, doctorAddress). The doctor securely retrieves the encrypted URI via getPrivateTokenURI.

🛠️ Deployment and Verification (Foundry & Xsolla)

Deployment on Sepolia

Your script (script/Deploy.s.sol) is set up to deploy the contract and set the minterServiceAddress and baseImageURI.
Bash

forge build
source .env # Ensure $SEPOLIA_RPC_URL and $PRIVATE_KEY are loaded
forge script script/Deploy.s.sol:DeployMedicalCard \
    --rpc-url $SEPOLIA_RPC_URL \
    --private-key $PRIVATE_KEY \
    --broadcast \
    --verify

Xsolla ZK Sepolia Verification (Crucial for Trust)

Verification confirms the deployed code matches the source code. Since Xsolla ZK Sepolia uses a custom explorer, you must follow their specific API requirements.

    Generate Constructor Arguments (Hex): Accurately encode the initial arguments (Owner, Name, Symbol) used during deployment.
    Bash

cast abi-encode "constructor(address,string,string)" <DEPLOYER_ADDRESS> "Xsolla Medical Card NFT" "xMCARD" | sed 's/^0x//'

Flatten Source Code: Create a single-file version for the verifier.
Bash

    forge flatten src/MedicalCard.sol > MedicalCard.flattened.sol

    Submit via Curl (Recommended): Use the Xsolla API endpoint defined in your environment variable to submit the flattened source and constructor args. Check Xsolla's documentation for the exact API fields.

Pro-Tip: If verification fails, ensure the compiler version (0.8.30) and constructor arguments match exactly what was used for deployment.