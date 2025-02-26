# Based Cheshire Trading Terminal Bot: Quick Start Guide 🐱

This guide will help you get started with the Based Cheshire Trading Terminal Bot quickly and efficiently.

## 🚀 Quick Setup

### 1. Prerequisites
- Node.js v16 or higher
- Telegram account
- Base network wallet with ETH
- Text editor (VSCode recommended)

### 2. Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/Based-Chesh-Trading-Terminal-Bot.git

# Navigate to project directory
cd Based-Chesh-Trading-Terminal-Bot

# Install dependencies
npm install
```

### 3. Configuration

1. Create a `.env` file in the root directory:
```bash
cp .env.example .env
```

2. Obtain the following API keys:

#### Telegram Bot
1. Message [@BotFather](https://t.me/BotFather) on Telegram
2. Send `/newbot`
3. Follow instructions to create bot
4. Copy the API token to `TELEGRAM_BOT_TOKEN`

#### Groq API
1. Visit [Groq Console](https://console.groq.com)
2. Create an account and get API key
3. Add to `GROQ_API_KEY`

#### OpenAI API
1. Visit [OpenAI Platform](https://platform.openai.com)
2. Create account/Sign in
3. Get API key
4. Add to `OPENAI_API_KEY`

#### Pinata (IPFS)
1. Visit [Pinata](https://app.pinata.cloud)
2. Create account
3. Get API key and Gateway key
4. Add to `PINATA_API_KEY` and `PINATA_GATEWAY_KEY`

#### Birdeye API
1. Visit [Birdeye](https://birdeye.so)
2. Register for API access
3. Add key to `BIRDEYE_API_KEY`

#### Base Network
1. Get Base RPC URL from [Coinbase Cloud](https://www.coinbase.com/cloud)
2. Add to `BASE_RPC_URL`

#### Basescan API
1. Visit [Basescan](https://basescan.org)
2. Create account
3. Get API key
4. Add to `BASESCAN_API_KEY`

### 4. Start the Bot

```bash
# Start the bot
node index.js
```

## 🎮 Basic Usage

### 1. Initial Setup
1. Open Telegram
2. Search for your bot username
3. Send `/start`
4. View available commands

### 2. Create Wallet
1. Click "Create Wallet" button
2. Save provided address
3. Fund wallet with Base ETH

### 3. Generate Art
1. Click "Generate Art" button
2. Choose DALL-E 3 or SDXL
3. Enter your prompt
4. Wait for generation
5. Use `/nft` to mint if desired

### 4. Check Portfolio
1. Click "Check Portfolio"
2. Enter wallet address
3. View holdings and analysis

### 5. Use AI Features
1. Chat with AI
   - Click "Chat with Groq"
   - Ask any crypto/DeFi question
   - Get AI-powered responses

2. Analyze Images
   - Click "Vision Analysis" or use /vision
   - Provide image URL and question
   - Get detailed AI analysis of charts and images

## 🛠 Common Operations

### Vision Analysis
```
1. Analyze Charts
   - Click "Vision Analysis"
   - Enter image URL and question
   - Format: image_url | question
   - Wait for AI analysis

2. Example Usage
   - Trading Charts: "What's the trend in this chart?"
   - NFT Analysis: "Describe this NFT artwork"
   - Technical Analysis: "What patterns do you see?"
```


### Managing ETH
```
1. Deposit ETH
   - Click "Deposit ETH"
   - Send ETH to provided address

2. Check Balance
   - Click "Check Balance"
   - View current ETH balance

3. Withdraw ETH
   - Click "Withdraw ETH"
   - Enter amount and address
   - Confirm transaction
```

### NFT Operations
```
1. Generate Art
   - Click "Generate Art"
   - Choose model
   - Enter prompt
   - Wait for generation

2. Mint NFT
   - Use /nft command
   - Provide image URL, name, description
   - Wait for minting
   - View on Base explorer
```

### Market Analysis
```
1. Check Token Price
   - Click "Token Price"
   - Enter token address
   - View price data

2. View Trending
   - Click "Trending"
   - See top tokens
   - View market data
```

## 🔧 Troubleshooting

### Common Issues

1. Bot Not Responding
```
- Check internet connection
- Verify bot is running
- Ensure valid API keys
```

2. Transaction Failures
```
- Check ETH balance
- Verify gas settings
- Confirm network status
```

3. NFT Generation Issues
```
- Check prompt guidelines
- Verify API keys
- Ensure stable connection
```

### Error Messages

1. "Invalid API Key"
```
- Verify all API keys in .env
- Check for whitespace
- Regenerate if needed
```

2. "Insufficient Funds"
```
- Add more ETH to wallet
- Check gas prices
- Adjust transaction amount
```

3. "Generation Failed"
```
- Check API status
- Verify prompt content
- Try different model
```

## 📱 Command Reference

### Basic Commands
- `/start` - Initialize bot
- `/help` - Show help menu
- `/generate` - Start art generation
- `/nft` - Begin NFT minting

### Wallet Commands
- `Check Balance` - View ETH balance
- `Deposit ETH` - Get deposit address
- `Withdraw ETH` - Send ETH out
- `Export Key` - Backup wallet

### Trading Commands
- `Token Price` - Check prices
- `Trending` - View top tokens
- `Buy Tokens` - Purchase tokens
- `Sell Tokens` - Sell tokens

### NFT Commands
- `Generate Art` - Create AI art
- `Mint NFT` - Create NFT
- Format: `image_url | name | description`

## 🔒 Security Best Practices

1. Private Key Safety
```
- Never share private keys
- Use strong passwords
- Enable encryption
```

2. Transaction Safety
```
- Verify addresses
- Start with small amounts
- Check gas prices
```

3. API Key Protection
```
- Secure .env file
- Regular key rotation
- Monitor usage
```

## 🆘 Getting Help

### Support Channels
1. GitHub Issues
2. Telegram Support
3. Documentation

### Reporting Bugs
1. Describe the issue
2. Provide error messages
3. List steps to reproduce
4. Include environment details

## 🚀 Next Steps

1. Explore Advanced Features
- Try AI chat
- Generate custom NFTs
- Analyze portfolios

2. Join Community
- Follow updates
- Share feedback
- Contribute ideas

3. Stay Updated
- Check for updates
- Read documentation
- Follow roadmap

Remember: Always prioritize security and start with small transactions until you're comfortable with the system.

