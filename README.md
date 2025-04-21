# Web3 Crowd Funding Platform

This is a decentralized crowdfunding platform built using Next.js, TailwindCSS, and the Thirdweb SDK. The platform allows users to create and manage crowdfunding campaigns on the blockchain.

## Features

- **Campaign Management**: Create, view, and manage crowdfunding campaigns.
- **Funding Tiers**: Add and manage funding tiers for campaigns.
- **Wallet Integration**: Connect your wallet to interact with the platform.
- **Blockchain Integration**: All campaigns and transactions are managed on the blockchain using Thirdweb.

## Tech Stack

- **Frontend**: Next.js, React, TailwindCSS
- **Blockchain SDK**: Thirdweb
- **Smart Contracts**: Solidity (via Thirdweb)

## Prerequisites

To run this project, ensure you have the following installed:

- Node.js (v16 or later)
- Yarn (or npm)

## Environment Variables

Create a `.env` file in the root directory and add the following environment variables:

```
NEXT_PUBLIC_TEMPLATE_CLIENT_ID=<Your Thirdweb Client ID>
```

Refer to the [Thirdweb documentation](https://portal.thirdweb.com/typescript/v5/client) for details on obtaining a client ID.

## Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd web3-crowd-funding
```

### 2. Install Dependencies

```bash
yarn
```

### 3. Run the Development Server

```bash
yarn dev
```

The application will be available at `http://localhost:3000`.

### 4. Build for Production

```bash
yarn build
```

### 5. Preview the Production Build

```bash
yarn start
```

## Project Structure

```
web3-crowd-funding/
├── public/                # Static assets
├── src/
│   ├── app/              # Next.js app directory
│   │   ├── campaign/     # Campaign-related pages
│   │   ├── dashboard/    # Dashboard pages
│   │   ├── constants/    # Constants (e.g., contract addresses)
│   │   ├── client.ts     # Thirdweb client setup
│   │   ├── globals.css   # Global styles
│   │   ├── layout.tsx    # Root layout
│   │   └── page.tsx      # Home page
│   ├── components/       # Reusable UI components
├── tailwind.config.ts     # TailwindCSS configuration
├── tsconfig.json          # TypeScript configuration
├── next.config.mjs        # Next.js configuration
├── package.json           # Project dependencies and scripts
└── README.md              # Project documentation
```

## Smart Contracts

The platform interacts with smart contracts deployed on the blockchain. The contract addresses are defined in `src/app/constants/contracts.ts`.

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push the branch.
4. Open a pull request.

## Acknowledgments

- [Thirdweb](https://thirdweb.com/) for the blockchain SDK.
- [Next.js](https://nextjs.org/) for the React framework.
- [TailwindCSS](https://tailwindcss.com/) for styling.