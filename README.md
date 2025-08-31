# 🚀 BRC-20 Smart Contract Platform

> **A revolutionary full-stack platform bridging Bitcoin and Ethereum ecosystems**

A comprehensive smart contract platform that seamlessly integrates BRC-20 token functionality with traditional Ethereum smart contracts. Built with enterprise-grade architecture featuring a TypeScript backend with advanced Bitcoin/PSBT integration and a modern, responsive Next.js frontend.

## ✨ Key Highlights

- 🔗 **Cross-Chain Integration**: Seamlessly bridge Bitcoin and Ethereum ecosystems
- 🎯 **BRC-20 Native**: Built specifically for Bitcoin Ordinals and BRC-20 tokens
- 🛡️ **Enterprise Security**: Multi-signature wallets, PSBT support, and secure key management
- ⚡ **High Performance**: Optimized TypeScript backend with real-time blockchain interactions
- 🎨 **Modern UI/UX**: Beautiful, responsive interface built with Next.js 14 and NextUI

## 🏗️ Project Structure

```
code/
├── be/                     # Backend (Node.js + TypeScript)
│   ├── config/            # Configuration files
│   ├── controller/        # Route controllers
│   ├── middleware/        # Express middleware
│   ├── model/            # Data models
│   ├── routes/           # API routes
│   ├── service/          # Business logic services
│   ├── utils/            # Utility functions
│   ├── output/           # Smart contract artifacts
│   ├── Simple.sol        # Solidity smart contract
│   └── wallet.json       # Bitcoin wallet configuration
├── fe/                    # Frontend (Next.js + React)
│   ├── app/              # Next.js app directory
│   ├── components/       # React components
│   ├── contexts/         # React contexts
│   └── utils/            # Frontend utilities
└── README.md
```

## 🚀 Core Features

### 🔧 Backend Capabilities
| Feature | Description |
|---------|-------------|
| **Bitcoin Integration** | Full PSBT (Partially Signed Bitcoin Transaction) support with advanced signing workflows |
| **BRC-20 Token Support** | Native BRC-20 token deployment, minting, and management |
| **Smart Contract Engine** | Solidity contract compilation, deployment, and interaction |
| **Multi-Signature Wallets** | Taproot and traditional multisig with flexible signing policies |
| **Inscription Management** | Bitcoin inscription creation, transfer, and OP_RETURN operations |
| **RUNE Protocol** | Integration with Bitcoin Runes for enhanced token functionality |

### 🎨 Frontend Experience
| Feature | Description |
|---------|-------------|
| **Modern Architecture** | Next.js 14 with App Router and TypeScript |
| **UI Components** | NextUI + Tailwind CSS for beautiful, responsive design |
| **Wallet Integration** | Support for Unisat, Sats Connect, and other Bitcoin wallets |
| **Real-time Updates** | Live blockchain transaction monitoring and state updates |
| **Mobile-First** | Responsive design optimized for all device sizes |

### 📜 Smart Contract Features
| Feature | Description |
|---------|-------------|
| **Custom BRC-20 Contract** | `Custom_Simple_Brc2_0` with advanced value storage and management |
| **Cross-Chain Compatibility** | Deploy to Ethereum and Bitcoin-compatible networks |
| **State Management** | Persistent storage with get/set value operations |
| **Gas Optimization** | Efficient contract design for cost-effective operations |

## 🛠️ Technology Stack

### 🔧 Backend Technologies
| Category | Technology | Version | Purpose |
|----------|------------|---------|---------|
| **Runtime** | Node.js + TypeScript | 18+ | Server-side execution |
| **Framework** | Express.js | 4.18+ | Web application framework |
| **Bitcoin** | bitcoinjs-lib | 6.1+ | Bitcoin transaction handling |
| **Bitcoin** | @unisat/ord-utils | Latest | Ordinal and inscription support |
| **Bitcoin** | runelib | 1.0+ | Bitcoin Runes integration |
| **Ethereum** | ethers.js | 6.15+ | Smart contract interaction |
| **Ethereum** | solc | 0.8.30 | Solidity compilation |
| **Database** | MongoDB + Mongoose | 8.0+ | Data persistence |
| **Security** | JWT + bcryptjs | Latest | Authentication & encryption |
| **Validation** | express-validator | 7.0+ | Input validation |

### 🎨 Frontend Technologies
| Category | Technology | Version | Purpose |
|----------|------------|---------|---------|
| **Framework** | Next.js | 14.1+ | React framework with SSR |
| **Language** | TypeScript | 5.0+ | Type-safe development |
| **UI Library** | NextUI | 2.2+ | Modern component library |
| **Styling** | Tailwind CSS | 3.3+ | Utility-first CSS framework |
| **State** | React Context | 18.2+ | Global state management |
| **Wallets** | Sats Connect | 1.4+ | Bitcoin wallet integration |
| **Wallets** | Unisat Utils | 1.0+ | Advanced wallet features |
| **Icons** | React Icons | 5.1+ | Icon library |
| **Notifications** | React Toastify | 10.0+ | User feedback system |

## 📋 Prerequisites

### System Requirements
| Requirement | Version | Description |
|-------------|---------|-------------|
| **Node.js** | 18.0.0+ | JavaScript runtime environment |
| **npm/yarn** | Latest | Package manager |
| **Git** | 2.0+ | Version control system |

### Optional Dependencies
| Dependency | Purpose | Installation |
|------------|---------|--------------|
| **Bitcoin Core** | Local Bitcoin network | [Download](https://bitcoin.org/en/download) |
| **MongoDB** | Local database | [Install Guide](https://docs.mongodb.com/manual/installation/) |
| **Docker** | Containerized development | [Get Docker](https://docs.docker.com/get-docker/) |

## ⚡ Quick Start

### 🚀 1. Clone & Setup
```bash
# Clone the repository
git clone <repository-url>
cd code

# Install dependencies for both projects
npm run setup:all
```

### 🔧 2. Backend Configuration
```bash
cd be
npm install
```

**Environment Configuration** - Create `.env` file:
```env
# Server Configuration
PORT=3001
NODE_ENV=development

# Database
MONGO_URI=mongodb://localhost:27017/brc20-platform

# Security
JWT_SECRET=your_super_secure_jwt_secret_here
JWT_EXPIRES_IN=24h

# Bitcoin Configuration
TEST_MODE=true
BITCOIN_NETWORK=testnet

# External APIs
UNISAT_API_URL=https://open-api-signet.unisat.io
MEMPOOL_API_URL=https://mempool.space/testnet/api

# Optional: Bitcoin Core RPC
BITCOIN_RPC_HOST=127.0.0.1
BITCOIN_RPC_PORT=38332
BITCOIN_RPC_USER=your_rpc_username
BITCOIN_RPC_PASSWORD=your_rpc_password
```

**Start Backend Services**:
```bash
npm run dev      # Development with hot reload
npm run build    # Production build
npm start        # Production mode
npm run test     # Run test suite
```

### 🎨 3. Frontend Configuration
```bash
cd fe
npm install
```

**Environment Configuration** - Create `.env.local` file:
```env
# API Configuration
NEXT_PUBLIC_API_URL=http://localhost:3001
NEXT_PUBLIC_NETWORK=testnet

# Wallet Configuration
NEXT_PUBLIC_DEFAULT_WALLET=unisat
NEXT_PUBLIC_CHAIN_ID=1

# Feature Flags
NEXT_PUBLIC_ENABLE_ANALYTICS=false
NEXT_PUBLIC_ENABLE_DEBUG=true
```

**Start Frontend Services**:
```bash
npm run dev      # Development server
npm run build    # Production build
npm start        # Production server
npm run lint     # Code quality check
```

### 🌐 4. Access Your Application
| Service | URL | Description |
|---------|-----|-------------|
| **Frontend** | http://localhost:3000 | Main application interface |
| **Backend API** | http://localhost:3001 | REST API endpoints |
| **API Docs** | http://localhost:3001/api-docs | Swagger documentation |
| **Health Check** | http://localhost:3001/health | Service status |

## 🔧 Configuration Guide

### 🌐 Network Configuration
| Network | TEST_MODE | Use Case | API Endpoints |
|---------|-----------|----------|---------------|
| **Testnet** | `true` | Development & Testing | Signet, Testnet APIs |
| **Mainnet** | `false` | Production | Mainnet APIs |

**Environment Variables**:
```env
# Bitcoin Network
TEST_MODE=true                    # true=testnet, false=mainnet
BITCOIN_NETWORK=testnet          # testnet, mainnet, signet
UNISAT_API_URL=https://open-api-signet.unisat.io  # Testnet
# UNISAT_API_URL=https://open-api.unisat.io       # Mainnet
```

### 📜 Smart Contract Configuration
Smart contracts are automatically compiled and deployed through our API endpoints. All artifacts are stored in `be/output/`:

| File | Purpose | Generated When |
|------|---------|----------------|
| `Simple_deploy_tx.json` | Contract deployment data | Contract deployment |
| `Simple_setValue_tx.json` | Value setting transaction | Value modification |
| `Simple_getValue_tx.json` | Value retrieval data | Value querying |
| `Simple.abi` | Contract interface | Contract compilation |
| `Simple.bytecode` | Compiled contract | Contract compilation |

### 🔐 Security Configuration
| Setting | Description | Recommendation |
|---------|-------------|----------------|
| `JWT_SECRET` | Authentication secret | Use 64+ character random string |
| `JWT_EXPIRES_IN` | Token expiration | 24h for development, 1h for production |
| `CORS_ORIGIN` | Allowed origins | Restrict to your domains |
| `RATE_LIMIT` | API rate limiting | Enable in production |

## 📚 API Reference

### 🔧 Smart Contract Endpoints
| Endpoint | Method | Description | Request Body |
|----------|--------|-------------|--------------|
| `/deploy-inscription` | `POST` | Deploy smart contract and create inscription | `{paymentAddress, ordinalAddress}` |
| `/get-value-inscription` | `POST` | Get value from smart contract | `{paymentAddress, ordinalAddress}` |
| `/set-value-inscription` | `POST` | Set value in smart contract | `{paymentAddress, ordinalAddress, value}` |
| `/transfer-to-opreturn` | `POST` | Transfer inscription to OP_RETURN | `{paymentAddress, ordinalAddress}` |
| `/get-value-from-smart-contract` | `GET` | Query contract state | Query parameters |

### ₿ Bitcoin/PSBT Endpoints
| Endpoint | Method | Description | Request Body |
|----------|--------|-------------|--------------|
| `/final-sign` | `POST` | Finalize and broadcast Bitcoin transaction | `{psbt, signatures}` |
| `/pre-sign` | `POST` | Prepare Bitcoin transaction for signing | `{inputs, outputs, fee}` |

### 📊 Response Format
All API endpoints return a consistent response format:
```json
{
  "success": true,
  "message": "Operation completed successfully",
  "payload": {
    // Response data specific to the endpoint
  }
}
```

### 🔍 Error Handling
```json
{
  "success": false,
  "message": "Error description",
  "payload": {
    "error": "Detailed error information",
    "code": "ERROR_CODE"
  }
}
```

## 🔐 Security & Best Practices

### 🛡️ Security Features
| Feature | Description | Implementation |
|---------|-------------|----------------|
| **Wallet Security** | Private keys and wallet files are gitignored | `.gitignore` configuration |
| **Environment Variables** | Sensitive data stored in environment files | `.env` files with gitignore |
| **CORS Protection** | Configurable cross-origin resource sharing | Express CORS middleware |
| **Input Validation** | Request data validation and sanitization | Express validator middleware |
| **JWT Authentication** | Secure API authentication with tokens | JWT + bcryptjs |
| **Rate Limiting** | API request rate limiting | Express rate-limit |
| **Helmet Security** | Security headers for Express | Helmet middleware |

### 🔒 Security Recommendations
```bash
# Generate secure JWT secret
node -e "console.log(require('crypto').randomBytes(64).toString('hex'))"

# Use strong passwords for Bitcoin RPC
# Minimum 16 characters with special characters

# Enable HTTPS in production
# Use Let's Encrypt for free SSL certificates
```

## 🧪 Testing & Quality Assurance

### 🔧 Backend Testing
```bash
cd be

# Run all tests
npm run test

# Run tests with coverage
npm run test:coverage

# Run tests in watch mode
npm run test:watch

# Run specific test file
npm run test -- routes/test/index.test.ts
```

### 📜 Smart Contract Testing
The platform includes comprehensive testing for smart contract functionality:

| Test Type | Description | Endpoint |
|-----------|-------------|----------|
| **Contract Deployment** | Verify contract compilation and deployment | `/deploy-inscription` |
| **Value Operations** | Test set/get value functions | `/set-value-inscription`, `/get-value-inscription` |
| **Transaction Broadcasting** | Verify transaction finalization | `/final-sign` |
| **OP_RETURN Operations** | Test inscription transfers | `/transfer-to-opreturn` |

### 🧪 Test Coverage
```bash
# Generate coverage report
npm run test:coverage

# View coverage in browser
open coverage/lcov-report/index.html
```

### 🔍 Manual Testing
```bash
# Test API endpoints
curl -X POST http://localhost:3001/deploy-inscription \
  -H "Content-Type: application/json" \
  -d '{"paymentAddress":"bc1...","ordinalAddress":"bc1..."}'

# Test smart contract interaction
curl -X GET http://localhost:3001/get-value-from-smart-contract
```

## 🚀 Deployment Guide

### 🔧 Backend Deployment

#### 1. Production Build
```bash
cd be

# Install production dependencies
npm ci --only=production

# Build TypeScript project
npm run build

# Verify build output
ls -la dist/
```

#### 2. Server Deployment
```bash
# Copy build files to server
scp -r dist/ user@your-server:/var/www/brc20-backend/
scp package.json user@your-server:/var/www/brc20-backend/
scp .env.production user@your-server:/var/www/brc20-backend/.env

# On server
cd /var/www/brc20-backend
npm ci --only=production
npm start
```

#### 3. Environment Configuration
```env
# Production .env
NODE_ENV=production
PORT=3001
MONGO_URI=mongodb://production-db:27017/brc20-platform
JWT_SECRET=your_production_jwt_secret
TEST_MODE=false
BITCOIN_NETWORK=mainnet
```

### 🎨 Frontend Deployment

#### 1. Build Application
```bash
cd fe

# Install dependencies
npm ci

# Build for production
npm run build

# Verify build output
ls -la .next/
```

#### 2. Deploy Options

**Option A: Vercel (Recommended)**
```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
```

**Option B: Static Export**
```bash
# Add to next.config.mjs
const nextConfig = {
  output: 'export',
  trailingSlash: true,
}

# Build and export
npm run build
# Static files in out/ directory
```

**Option C: Traditional Hosting**
```bash
# Copy build files
scp -r .next/ user@your-server:/var/www/brc20-frontend/
scp -r public/ user@your-server:/var/www/brc20-frontend/

# Configure nginx/Apache to serve static files
```

### 🐳 Docker Deployment
```dockerfile
# Backend Dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm ci --only=production
COPY dist/ ./dist/
EXPOSE 3001
CMD ["npm", "start"]
```

```bash
# Build and run
docker build -t brc20-backend .
docker run -p 3001:3001 brc20-backend
```

## 🤝 Contributing

We welcome contributions from the community! Here's how you can help improve the BRC-20 Smart Contract Platform.

### 🚀 Getting Started
1. **Fork the repository** to your GitHub account
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/your-username/brc20-platform.git
   cd brc20-platform
   ```
3. **Add upstream remote**:
   ```bash
   git remote add upstream https://github.com/original-owner/brc20-platform.git
   ```

### 🔧 Development Workflow
```bash
# Create feature branch
git checkout -b feature/amazing-feature

# Make your changes
# ... edit files ...

# Commit with conventional commits
git commit -m "feat: add amazing new feature"

# Push to your fork
git push origin feature/amazing-feature

# Create Pull Request
```

### 📝 Commit Guidelines
We use [Conventional Commits](https://www.conventionalcommits.org/):
- `feat:` New features
- `fix:` Bug fixes
- `docs:` Documentation changes
- `style:` Code style changes
- `refactor:` Code refactoring
- `test:` Adding tests
- `chore:` Maintenance tasks

### 🧪 Testing Requirements
- All new features must include tests
- Ensure all existing tests pass
- Maintain or improve test coverage

### 📋 Pull Request Checklist
- [ ] Code follows project style guidelines
- [ ] Tests pass locally
- [ ] Documentation is updated
- [ ] Commit messages follow conventional format
- [ ] No sensitive data is exposed

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🐛 Troubleshooting Guide

### ❌ Common Issues & Solutions

#### 1. **"Cannot convert undefined to BigInt" Error**
**Problem**: Smart contract call returns undefined result
```bash
TypeError: Cannot convert undefined to a BigInt
```

**Solutions**:
- ✅ Verify smart contract is deployed and accessible
- ✅ Check contract address in API calls
- ✅ Ensure network configuration matches contract deployment
- ✅ Verify function selector is correct (`0x20965255` for `getValue()`)

**Debug Steps**:
```bash
# Check contract deployment
curl -X GET http://localhost:3001/get-value-from-smart-contract

# Verify network configuration
echo $TEST_MODE
echo $BITCOIN_NETWORK
```

#### 2. **Bitcoin RPC Connection Issues**
**Problem**: Cannot connect to Bitcoin Core RPC
```bash
Error: connect ECONNREFUSED 127.0.0.1:38332
```

**Solutions**:
- ✅ Verify Bitcoin Core is running: `bitcoin-cli getblockchaininfo`
- ✅ Check RPC credentials in environment variables
- ✅ Ensure proper network configuration (testnet/mainnet)
- ✅ Verify RPC port is open and accessible

**Debug Steps**:
```bash
# Test Bitcoin Core connection
bitcoin-cli -testnet getblockchaininfo

# Check RPC configuration
grep -r "rpc" ~/.bitcoin/bitcoin.conf
```

#### 3. **Smart Contract Compilation Errors**
**Problem**: Solidity compilation fails
```bash
Error: Invalid Solidity version or syntax error
```

**Solutions**:
- ✅ Verify Solidity version compatibility (^0.8.0)
- ✅ Check contract syntax in `Simple.sol`
- ✅ Ensure solc compiler is properly installed
- ✅ Verify all dependencies are installed

**Debug Steps**:
```bash
# Check Solidity version
solc --version

# Verify contract syntax
solc --strict-imports Simple.sol
```

#### 4. **JSON File Reading Issues**
**Problem**: Cannot read smart contract artifacts
```bash
Error: JSON file is empty or not found
```

**Solutions**:
- ✅ Ensure contract compilation completed successfully
- ✅ Check file paths and permissions
- ✅ Verify `be/output/` directory exists
- ✅ Check for file corruption or truncation

### 🔍 Getting Help

#### **Before Creating an Issue**
1. **Check existing issues** for similar problems
2. **Search documentation** for solutions
3. **Verify your setup** matches requirements
4. **Test with minimal configuration**

#### **Creating a Helpful Issue**
```markdown
**Environment**:
- OS: [e.g., Windows 10, Ubuntu 20.04]
- Node.js: [e.g., v18.17.0]
- Network: [e.g., testnet, mainnet]

**Error Details**:
- Full error message
- Stack trace
- Steps to reproduce

**Configuration**:
- Relevant environment variables
- Network settings
- Contract addresses

**Additional Context**:
- What you were trying to do
- What you expected to happen
- Any recent changes made
```

#### **Community Resources**
- 📖 [Documentation](link-to-docs)
- 💬 [Discord Community](link-to-discord)
- 🐛 [GitHub Issues](link-to-issues)
- 📚 [Wiki](link-to-wiki)

## 🔗 Related Projects & Resources

### 🏗️ Core Technologies
| Project | Description | Link |
|---------|-------------|------|
| **bitcoinjs-lib** | Bitcoin library for JavaScript | [GitHub](https://github.com/bitcoinjs/bitcoinjs-lib) |
| **ethers.js** | Ethereum library for smart contracts | [GitHub](https://github.com/ethers-io/ethers.js/) |
| **Next.js** | React framework with SSR | [Website](https://nextjs.org/) |
| **NextUI** | Modern React component library | [Website](https://nextui.org/) |

### 📚 Learning Resources
| Resource | Type | Description |
|----------|------|-------------|
| **Bitcoin Development** | Documentation | [Bitcoin Developer Guide](https://bitcoin.org/en/developer-documentation) |
| **BRC-20 Standard** | Specification | [BRC-20 Documentation](https://docs.ordinals.com/) |
| **Solidity** | Language | [Solidity Docs](https://docs.soliditylang.org/) |
| **PSBT** | Protocol | [BIP-174 Specification](https://github.com/bitcoin/bips/blob/master/bip-0174.mediawiki) |

### 🌐 Community & Support
| Platform | Purpose | Link |
|----------|---------|------|
| **Discord** | Community chat | [Join Server](link-to-discord) |
| **Telegram** | News & updates | [Channel](link-to-telegram) |
| **Twitter** | Announcements | [Follow](link-to-twitter) |
| **GitHub** | Source code | [Repository](link-to-repo) |

---

## 🏆 Acknowledgments

Special thanks to the open-source community and contributors who made this project possible:

- **Bitcoin Core Developers** - For the revolutionary blockchain technology
- **Ethereum Foundation** - For smart contract innovation
- **Open Source Contributors** - For building the tools we use
- **Community Members** - For testing, feedback, and support

---

**🚀 Made with ❤️ for the Bitcoin and Ethereum communities**

*Building the future of decentralized finance, one transaction at a time.*
