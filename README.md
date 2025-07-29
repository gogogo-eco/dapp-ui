# DATACOIN dApp Frontend

A modern, responsive web application for managing both native DTC and DTCERC tokens with MetaMask integration built with Next.js 15, React 19, TypeScript, and Tailwind CSS.

## 🪙 Token Architecture

This dApp supports two types of tokens on the DATACOIN network:

- **Native DTC**: The native currency of the DATACOIN network (like ETH on Ethereum)
- **DTCERC Token**: A custom ERC20 token with additional features (minting, burning, etc.)

## 🌟 Features

### 🔗 MetaMask Integration
- **Seamless Wallet Connection**: One-click MetaMask connection with automatic network detection
- **Network Management**: Automatic network switching to Ethermint with user-friendly prompts
- **Token Management**: Add DATACOIN token to MetaMask wallet automatically
- **Real-time Balance**: Live token balance updates with periodic refresh

### 💰 Token Operations
- **Send Tokens**: Transfer DATACOIN tokens to any Ethereum address with validation
- **Receive Tokens**: View incoming transactions and token receipts
- **Balance Tracking**: Real-time balance display with formatted amounts
- **Transaction History**: Complete transaction log with filtering and export capabilities

### 🛒 Purchase System
- **Credit Card Integration**: Buy tokens with credit card (Stripe integration ready)
- **Secure Payments**: PCI-compliant payment processing with automatic token minting
- **Order Management**: Complete purchase flow with order confirmation and receipts
- **Price Calculator**: Real-time price calculation with fees and total display

### 👨‍💼 Admin Panel
- **Token Minting**: Create new tokens and distribute to specific addresses
- **Token Burning**: Remove tokens from circulation permanently
- **Supply Management**: Monitor total supply and circulation metrics
- **Admin Controls**: Secure admin-only operations with proper validation

### 📊 Analytics & Monitoring
- **Dashboard**: Comprehensive overview of token stats and portfolio
- **Transaction History**: Detailed transaction log with search and filtering
- **Market Data**: Token price, market cap, and holder statistics
- **Export Features**: CSV export for transaction history and reports

### 🎨 User Experience
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Dark Mode Support**: Automatic dark/light theme switching
- **Loading States**: Smooth loading indicators and skeleton screens
- **Error Handling**: Comprehensive error messages and recovery options
- **Notifications**: Toast notifications for all user actions and events

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ and npm
- MetaMask browser extension
- Running Ethermint node (for local development)

### Installation

1. **Clone and Install**
   ```bash
   cd dapp-ui
   npm install
   ```

2. **Environment Setup**
   ```bash
   cp .env.local.example .env.local
   ```

   Edit `.env.local` with your configuration:
   ```env
   NEXT_PUBLIC_CONTRACT_ADDRESS=0xYourContractAddress
   NEXT_PUBLIC_CHAIN_ID=9000
   NEXT_PUBLIC_RPC_URL=http://127.0.0.1:8545
   NEXT_PUBLIC_API_BASE_URL=http://localhost:3001/api
   ```

3. **Start Development Server**
   ```bash
   npm run dev
   ```

4. **Open Application**
   Navigate to [http://localhost:3000](http://localhost:3000)
