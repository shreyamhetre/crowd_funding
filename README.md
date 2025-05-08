## Getting Started

Create a project using this example:

```bash
npx thirdweb create --template vite-javascript-starter
```

You can start editing the page by modifying `src/main.jsx`. The page auto-updates as you edit the file.

On `src/index.jsx`, you'll find our `ThirdwebProvider` wrapping your app,
this is necessary for our [hooks](https://portal.thirdweb.com/react) and
[UI Components](https://portal.thirdweb.com/ui-components) to work.

## Environment Variables

To run this project, you will need to add environment variables. Check the `.env.example` file for all the environment variables required and add it to `.env.local` file or set them up on your hosting provider.

### Deploy to IPFS

Deploy a copy of your application to IPFS using the following command:

```bash
yarn deploy
```

## Learn More

To learn more about thirdweb, Vite and React, take a look at the following resources:

- [thirdweb React Documentation](https://docs.thirdweb.com/react) - learn about our React SDK.
- [thirdweb JavaScript Documentation](https://docs.thirdweb.com/react) - learn about our JavaScript/TypeScript SDK.
- [thirdweb Portal](https://docs.thirdweb.com/react) - check our guides and development resources.
- [Vite Documentation](https://vitejs.dev/guide/) - learn about Vite features.
- [React documentation](https://reactjs.org/) - learn React.
- [Templates](https://thirdweb.com/templates)

You can check out [the thirdweb GitHub organization](https://github.com/thirdweb-dev) - your feedback and contributions are welcome!

## Join our Discord!

For any questions, suggestions, join our discord at [https://discord.gg/thirdweb](https://discord.gg/thirdweb).


## Crowd Funding DApp
## Overview
Crowd Funding DApp is a decentralized crowdfunding platform built on the Ethereum blockchain using the thirdweb SDK. It allows users to create, browse, and contribute to fundraising campaigns securely and transparently. The platform leverages smart contracts to ensure trustless transactions, eliminating intermediaries and enhancing transparency for backers and campaign creators.
---
## Objectives

Enable users to create crowdfunding campaigns with customizable goals, titles, and descriptions.
Allow global contributions to campaigns using Ethereum via MetaMask.
Ensure transparency through blockchain-based transaction records.
Provide a user-friendly interface for browsing and donating to campaigns.
Maintain security and decentralization using Ethereum smart contracts.
---
Features

Campaign Creation: Users can create campaigns by specifying a title, description, funding goal, and optional image.
Donation System: Contributors can donate ETH to campaigns using MetaMask, with transactions recorded on the blockchain.
Campaign Management: Creators can view and manage their campaigns, with funds securely held in smart contracts.
Responsive UI: Built with React and Tailwind CSS for a modern, mobile-friendly interface.
Decentralized Storage: Campaign data and metadata can be deployed to IPFS for persistent storage.

Technologies Used

Frontend: React, Vite, Tailwind CSS
Blockchain: Ethereum, thirdweb SDK, Solidity (smart contracts)
Wallet Integration: MetaMask
Deployment: IPFS (via thirdweb), Polygon Mumbai Testnet (for testing)
Languages: JavaScript, Solidity
Tools: Node.js, Yarn, Hardhat (for smart contract testing)

Repository Structure

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

Getting Started
Prerequisites

Node.js (v16 or higher)
Yarn (optional, can use npm)
MetaMask browser extension
An Ethereum wallet with testnet ETH (e.g., Polygon Mumbai Testnet)

Installation

Clone the repository:
git clone https://github.com/shreyamhetre/crowd_funding.git
cd crowd_funding


Install dependencies:
yarn install


Set up environment variables:

Copy .env.example to .env.local:cp .env.example .env.local


Update .env.local with the required variables:
VITE_THIRDWEB_CLIENT_ID: Your thirdweb client ID (get from thirdweb dashboard)
VITE_WALLET_CONNECT_PROJECT_ID: WalletConnect project ID (optional, for additional wallet support)
VITE_CONTRACT_ADDRESS: Address of the deployed smart contract (after deployment)




Deploy smart contracts (optional, for custom contracts):

Ensure Hardhat is configured in the project.
Compile and deploy contracts to the Polygon Mumbai Testnet:npx hardhat compile
npx hardhat run scripts/deploy.js --network mumbai


Update VITE_CONTRACT_ADDRESS in .env.local with the deployed contract address.


Run the application:
yarn dev


Open http://localhost:5173 in your browser to view the app.


Deploy to IPFS (optional):

Build and deploy the app to IPFS using thirdweb:yarn deploy


Follow the CLI prompts to publish to IPFS.



Usage

Connect Wallet: Use MetaMask to connect your Ethereum wallet to the app.
Create a Campaign: Navigate to the campaign creation page, fill in details (title, description, goal), and deploy the campaign.
Browse Campaigns: View active campaigns on the homepage, with details like progress and funding status.
Donate: Select a campaign, specify an ETH amount, and confirm the transaction via MetaMask.
Monitor Campaigns: Creators can track their campaigns, and backers can view their contributions.

Contribution
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature/your-feature).
Make your changes and commit (git commit -m "Add your feature").
Push to the branch (git push origin feature/your-feature).
Open a pull request with a detailed description of your changes.

Please ensure your code follows the project’s coding standards and includes tests where applicable.
License
This project is licensed under the MIT License. See the LICENSE file for details.
Learn More

thirdweb Documentation: Learn about the thirdweb SDK for blockchain integration.
Vite Documentation: Understand Vite’s features for fast development.
React Documentation: Explore React for building user interfaces.
Tailwind CSS Documentation: Style the app with Tailwind CSS.
thirdweb Templates: Discover more blockchain project templates.

Support
For questions or suggestions, join the thirdweb Discord or open an issue on the GitHub repository.

