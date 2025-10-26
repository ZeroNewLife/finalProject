# Medical Card NFT: Secure & Decentralized Health Records

This repository contains the smart contract and frontend for a decentralized medical card NFT system. The project prioritizes patient data privacy and ownership by storing sensitive medical records encrypted off-chain (IPFS/Pinata) while utilizing the NFT on-chain to manage strict access permissions (granting temporary access to doctors). The core goal is to provide secure and profitable decentralized health records.

## Key Features & Benefits

*   **Secure Data Storage:** Medical records are encrypted and stored off-chain on IPFS/Pinata, ensuring data privacy and security.
*   **NFT-Based Access Control:** NFTs are used to manage access permissions to patient records, granting temporary access to authorized doctors.
*   **Decentralized and Transparent:** Leverages blockchain technology for transparency and immutability.
*   **Patient Data Ownership:** Patients retain full control over their medical data and access permissions.
*   **Scalable Revenue Generation:** Potential for revenue through standard NFT minting mechanisms and access subscriptions.

## Prerequisites & Dependencies

*   **Foundry:** Blockchain development toolchain. [Installation Guide](https://book.getfoundry.sh/)
*   **Node.js:** JavaScript runtime environment. [Installation Guide](https://nodejs.org/)
*   **npm/yarn:** Package managers for JavaScript dependencies.
*   **Metamask or similar wallet:** For interacting with the blockchain.
*   **IPFS or Pinata account:** For storing encrypted medical records off-chain.

## Installation & Setup Instructions

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/ZeroNewLife/finalProject.git
    cd finalProject
    ```

2.  **Install Foundry dependencies:**

    ```bash
    forge install
    ```

3.  **Install frontend dependencies:**

    ```bash
    cd frontend
    npm install  # or yarn install
    cd ..
    ```

4.  **Configure environment variables:**

    *   Create a `.env` file in the root directory.
    *   Add the following variables, replacing the placeholders with your actual values:

    ```
    PRIVATE_KEY=<YOUR_WALLET_PRIVATE_KEY>
    RPC_URL=<YOUR_RPC_ENDPOINT>  (e.g., Infura, Alchemy)
    IPFS_GATEWAY=<YOUR_IPFS_GATEWAY> (Optional)
    PINATA_API_KEY=<YOUR_PINATA_API_KEY> (Optional)
    PINATA_API_SECRET=<YOUR_PINATA_API_SECRET> (Optional)

    ```

    *   **Security Note:** Never commit your private key to the repository. Use environment variables to keep it safe.

5.  **Deploy the smart contract:**

    ```bash
    forge script script/Deploy.s.sol --rpc-url $RPC_URL --private-key $PRIVATE_KEY --broadcast --verify
    ```

    *   Replace `$RPC_URL` and `$PRIVATE_KEY` with your configured values.
    *   Note the deployed contract address.

6.  **Configure the frontend:**

    *   Open `frontend/index.html` in your text editor.
    *   Update the `contractAddress` variable with the address of your deployed contract.
    *   Update the `rpcUrl` variable with your RPC endpoint (if necessary).

7.  **Run the frontend:**

    ```bash
    cd frontend
    npm run start # or yarn start
    ```

    This will typically start a development server at `http://localhost:3000`.

## Usage Examples

The frontend provides a user interface for:

*   Minting medical card NFTs.
*   Uploading encrypted medical records to IPFS/Pinata.
*   Granting and revoking access permissions to doctors.
*   Viewing medical records (if authorized).

## Configuration Options

*   **Contract Address:** The address of the deployed `MedicalCard.sol` contract.
*   **RPC URL:** The URL of the Ethereum RPC endpoint.
*   **IPFS Gateway:** The URL of the IPFS gateway used for retrieving medical records.  Defaults to a public gateway if not specified.
*   **Pinata API Key/Secret:** Required if you are using Pinata to store medical records.

## Contributing Guidelines

1.  Fork the repository.
2.  Create a new branch for your feature or bug fix.
3.  Make your changes and commit them with descriptive commit messages.
4.  Submit a pull request.

## License Information

Not specified.  Please contact the repository owner, ZeroNewLife, to clarify licensing terms.

## Acknowledgments

*   The Foundry framework.
*   The IPFS and Pinata services.
*   All contributors to the project.

## Project Structure
```
└── .github/
└── workflows/
├── test.yml
├── .gitignore
├── .gitmodules
├── README.md
└── broadcast/
└── Deploy.s.sol/
└── 555776/
├── run-1761410002154.json
├── run-latest.json
├── foundry.lock
├── foundry.toml
└── frontend/
├── index.html
└── lib/
└── script/
├── Deploy.s.sol
└── src/
├── MedicalCard.sol
