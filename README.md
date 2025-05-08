## Crowd Funding DApp
## Overview
Crowd Funding DApp is a decentralized crowdfunding platform built on the Ethereum blockchain using the thirdweb SDK. It allows users to create, browse, and contribute to fundraising campaigns securely and transparently. The platform leverages smart contracts to ensure trustless transactions, eliminating intermediaries and enhancing transparency for backers and campaign creators.

## Objectives
- Enable users to create crowdfunding campaigns with customizable goals, titles, and descriptions.
- Allow global contributions to campaigns using Ethereum via MetaMask.
- Ensure transparency through blockchain-based transaction records.
- Provide a user-friendly interface for browsing and donating to campaigns.
- Maintain security and decentralization using Ethereum smart contracts.

## Features
- Campaign Creation: Users can create campaigns by specifying a title, description, funding goal, and optional image.
- Donation System: Contributors can donate ETH to campaigns using MetaMask, with transactions recorded on the blockchain.
- Campaign Management: Creators can view and manage their campaigns, with funds securely held in smart contracts.
- Responsive UI: Built with React and Tailwind CSS for a modern, mobile-friendly interface.
- Decentralized Storage: Campaign data and metadata can be deployed to IPFS for persistent storage.

## Technologies Used
- Frontend: React, Vite, Tailwind CSS
- Blockchain: Ethereum, thirdweb SDK, Solidity (smart contracts)
- Wallet Integration: MetaMask
- Deployment: IPFS (via thirdweb), Polygon Mumbai Testnet (for testing)
- Languages: JavaScript, Solidity
- Tools: Node.js, Yarn, Hardhat (for smart contract testing)

## Repository Structure

src/: Frontend source code
main.jsx: Entry point for the React application
index.jsx: Configures the ThirdwebProvider for blockchain interactions
components/: Reusable React components (e.g., campaign cards, forms)
pages/: Page components for home, campaign creation, and details
contracts/: Solidity smart contracts for campaign creation and funding
public/: Static assets (e.g., images, favicon)
.env.example: Template for environment variables
vite.config.js: Vite configuration for fast development and builds
package.json: Project dependencies and scripts

## Getting Started
**Prerequisites**
Node.js (v16 or higher)
Yarn (optional, can use npm)
MetaMask browser extension
An Ethereum wallet with testnet ETH (e.g., Polygon Mumbai Testnet)

**Installation**
**STEP 1:**
Clone the repository:
git clone https://github.com/shreyamhetre/crowd_funding.git
cd crowd_funding

**STEP 2:**
Install dependencies:
yarn install

**STEP 3:**
Set up environment variables:
Copy .env.example to .env.local:
  cp .env.example .env.local

**STEP 4:**
Update .env.local with the required variables:
  -VITE_THIRDWEB_CLIENT_ID: Your thirdweb client ID (get from thirdweb dashboard)
  -VITE_WALLET_CONNECT_PROJECT_ID: WalletConnect project ID (optional, for additional wallet support)
  -VITE_CONTRACT_ADDRESS: Address of the deployed smart contract (after deployment)

**STEP 4:**
Run the application:
yarn dev

**STEP 5:**
Open http://localhost:5173 in your browser to view the app.

## Usage
Connect Wallet: Use MetaMask to connect your Ethereum wallet to the app.
Create a Campaign: Navigate to the campaign creation page, fill in details (title, description, goal), and deploy the campaign.
Browse Campaigns: View active campaigns on the homepage, with details like progress and funding status.
Donate: Select a campaign, specify an ETH amount, and confirm the transaction via MetaMask.
Monitor Campaigns: Creators can track their campaigns, and backers can view their contributions.

## Contribution
Contributions are welcome! To contribute:
