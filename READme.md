# Based Cheshire Trading Terminal Bot 🐱

A sophisticated Telegram bot that combines AI-powered trading insights, NFT creation, and DeFi functionality on the Base network. This innovative bot serves as your all-in-one companion for navigating the Base DeFi ecosystem with style and intelligence.

## 🌟 Key Features

### 1. AI-Powered Chat & Vision
- Engage in intelligent conversations about DeFi, crypto markets, and trading strategies
- Get real-time insights and analysis powered by Groq's advanced language model
- Analyze images and charts using XAI Vision technology
- Ask questions about market trends, token analysis, and technical concepts

### 2. NFT Creation & Minting
- Generate unique AI art using DALL-E 3 or SDXL
- Automatic minting to Base mainnet
- IPFS integration for decentralized storage
- Full metadata support with attributes
- Direct minting to your wallet

### 3. Portfolio Management
- Real-time wallet balance tracking
- Token portfolio analysis
- Transaction history viewing
- Gas price monitoring
- Secure key management

### 4. DeFi Operations
- ETH deposits and withdrawals
- Token swapping capabilities (coming soon)
- Real-time gas fee estimation
- Secure transaction handling

### 5. Market Analysis
- Trending tokens tracking
- Real-time price updates
- Portfolio value tracking
- Market sentiment analysis
- Chart and image analysis with AI vision

## 🤖 Bot Commands

### Basic Commands
- `/start` - Initialize the bot and display the main menu
- `/help` - Display help information and command list
- `/vision` - Analyze images and charts with AI

### Chat & Analysis Commands
- `Chat with Groq` - Start an AI conversation about crypto and DeFi
- `Vision Analysis` - Analyze images and trading charts
- `Trending Tokens` - View current trending tokens on Base
- `Check Portfolio` - Analyze any wallet's holdings
- `Gas Price` - Check current Base network gas prices

### Vision Commands
- `Vision Analysis` - Analyze images and charts
  - Format: `image_url | question`
  - Example: `https://example.com/chart.jpg | What do you see in this trading chart?`

### Wallet Operations
- `Check Balance` - View your wallet balance
- `Deposit ETH` - Get your deposit address
- `Withdraw ETH` - Withdraw ETH to another address
- `Export Key` - Securely export your private key
- `Transaction History` - View your recent transactions

### NFT Commands
- `Generate NFT` - Create and mint an AI-generated NFT
  - Format: `prompt | name | description`
  - Example: `a mystical cat in cyberpunk style | Cyber Cheshire | A digital feline guardian`

### Trading Commands (Coming Soon)
- `Buy Tokens` - Purchase tokens using ETH
- `Sell Tokens` - Sell tokens back to ETH

## 🏗 Technical Architecture

### Core Components
1. **Telegram Bot Interface**
   - Built using the Grammy framework
   - Real-time updates and interactive buttons
   - Markdown formatting for beautiful messages

2. **AI Integration**
   - Groq API for intelligent conversations
   - DALL-E 3 and SDXL for NFT art generation
   - XAI Vision for image and chart analysis
   - Custom prompt engineering for optimal results

3. **Blockchain Integration**
   - Web3.js for Base network interaction
   - Custom wallet management system
   - Secure transaction handling

4. **Storage & Security**
   - IPFS via Pinata for decentralized storage
   - Encrypted private key management
   - Environment variable configuration

### External Services
- **Birdeye API**: Market data and token tracking
- **Basescan API**: Transaction and gas price monitoring
- **Pinata**: IPFS gateway and pinning
- **OpenAI**: DALL-E 3 image generation
- **XAI**: Vision model for image analysis
- **Hyperbolic**: SDXL image generation

## 🚀 Innovation Highlights

1. **AI-First Approach**
   - Combines multiple AI models (Groq + DALL-E + XAI Vision)
   - Natural language interaction for complex operations
   - AI-powered market analysis and insights
   - Advanced image and chart analysis

2. **Base Network Integration**
   - Native support for Base mainnet
   - Optimized gas handling
   - Real-time network monitoring

3. **NFT Innovation**
   - One-click AI art generation and minting
   - Multiple generation models (DALL-E 3 & SDXL)
   - Automated IPFS storage
   - Rich metadata and attributes

4. **Security Features**
   - Encrypted key management
   - Secure transaction signing
   - Rate limiting and error handling

## 🛠 Setup Instructions

1. **Prerequisites**
   - Node.js v16 or higher
   - Telegram account
   - Base network wallet with ETH

2. **Environment Setup**
   ```bash
   # Clone the repository
   git clone [repository-url]
   cd Based-Chesh-Trading-Terminal-Bot

   # Install dependencies
   npm install

   # Configure environment variables
   cp .env.example .env
   # Edit .env with your credentials
   ```

3. **Required API Keys**
   - Telegram Bot Token (from @BotFather)
   - Groq API Key
   - OpenAI API Key
   - XAI Vision API Key
   - Pinata API Keys
   - Birdeye API Key
   - Basescan API Key
   - Hyperbolic API Key

4. **Running the Bot**

   ### Standard Method
   ```bash
   # Start the bot
   node index.js
   ```

   ### Docker Method (Recommended for 24/7 Operation)
   ```bash
   # Build and start the container
   docker-compose up -d

   # View logs
   docker-compose logs -f

   # Stop the bot
   docker-compose down

   # Update and restart
   docker-compose down
   docker-compose build --no-cache
   docker-compose up -d
   ```

   The Docker setup includes:
   - Automatic restart on failure
   - Health checks
   - Log rotation
   - Timezone configuration
   - Persistent storage for user data
   - Resource monitoring

## 📈 Future Roadmap

1. **Enhanced Trading Features**
   - DEX integration for token swapping
   - Limit orders and automated trading
   - Portfolio rebalancing

2. **Advanced AI Features**
   - Market prediction models
   - Sentiment analysis
   - Custom trading strategies
   - Enhanced chart analysis

3. **Community Features**
   - Social trading
   - Community-driven NFT collections
   - Trading competitions
   - Shared chart analysis

## 🤝 Contributing

We welcome contributions! Please see our contributing guidelines for more details.

## 📝 License

This project is licensed under the ISC License.

## 🚀 Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn
- ngrok for local development
- Telegram Bot Token
- Required API Keys (see Configuration section)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/Based-Chesh-Trading-Terminal-Bot.git
cd Based-Chesh-Trading-Terminal-Bot
```

2. Install dependencies for all components:
```bash
# Frontend
cd frontend && npm install

# Bot API
cd ../bot-api && npm install

# WebSocket Server
cd ../websocket-server && npm install
```

3. Set up environment variables:
Create .env files in each directory (frontend/.env.local, bot-api/.env, websocket-server/.env) with the required variables.

### Configuration

Required Environment Variables:

1. Frontend (.env.local):
```env
NEXT_PUBLIC_PRIVY_APP_ID=your_privy_app_id
NEXT_PUBLIC_BOT_TOKEN=your_bot_token
NEXT_PUBLIC_BOT_USERNAME=your_bot_username
NEXT_PUBLIC_BIRDEYE_API_KEY=your_birdeye_api_key
NEXT_PUBLIC_WS_URL=ws://localhost:3001
```

2. Bot API (.env):
```env
BOT_TOKEN=your_bot_token
PORT=3002
BIRDEYE_API_KEY=your_birdeye_api_key
```

3. WebSocket Server (.env):
```env
PORT=3001
BIRDEYE_API_KEY=your_birdeye_api_key
```

### Running the Application

1. Start the WebSocket server:
```bash
cd websocket-server
npm run dev
```

2. Start the Bot API server:
```bash
cd bot-api
npm run dev
```

3. Start ngrok for Telegram webhook:
```bash
ngrok http 3002
```

4. Set up Telegram webhook:
```bash
curl -k "https://api.telegram.org/bot<YOUR_BOT_TOKEN>/setWebhook?url=<YOUR_NGROK_URL>/webhook"
```

5. Start the frontend:
```bash
cd frontend
npm run dev
```

## 📚 Architecture

### Component Overview
1. **Frontend (Next.js)**
   - Real-time trading interface
   - Token price charts
   - Portfolio management
   - Authentication handling

2. **Bot API Server**
   - Telegram bot integration
   - Command processing
   - User management
   - Trading operations

3. **WebSocket Server**
   - Real-time price updates
   - Live notifications
   - Market data streaming
   - Connection management

### Data Flow
1. User authenticates via Telegram through Privy
2. Frontend establishes WebSocket connection
3. Bot API processes Telegram commands
4. Real-time updates flow through WebSocket

## 🔒 Security Features
- Secure authentication via Privy
- Environment variable protection
- API key management
- Rate limiting
- Error handling and logging

## 🛠 API Integrations
- Birdeye API for market data
- Telegram Bot API
- Privy for authentication
- Base network integration

## 📈 Use Cases

### 1. Token Trading
- Real-time price monitoring
- Trade execution via Telegram
- Portfolio tracking
- Price alerts

### 2. Market Analysis
- Historical price data
- Technical indicators
- Market trends
- Volume analysis

### 3. Portfolio Management
- Asset tracking
- Performance metrics
- Transaction history
- Balance monitoring

## 🤝 Contributing
Contributions are welcome! Please read our contributing guidelines and submit pull requests to our repository.

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments
- Birdeye API for market data
- Telegram Bot API for messaging
- Privy for authentication
- Base network for blockchain infrastructure

## 📞 Support
For support, please join our Telegram group or create an issue in the repository.

## 🚀 Future Roadmap
1. Advanced trading features
2. Additional market data sources
3. Enhanced analytics
4. Mobile application
5. Extended Base network integration
