# Pi Masters: Royal Edition

A royal game of checkers powered by Pi Network.

## Configuration

Before running the game, you need to set up your Pi Network credentials:

1. Create a `.env` file in the root directory (copy from `.env.example`)
2. Fill in the following environment variables:

   ```env
   VITE_PI_API_KEY=your_api_key_here        # Get this from Pi Developer Portal
   VITE_MERCHANT_WALLET=your_wallet_address  # Your Pi wallet address
   VITE_PI_SANDBOX=true                      # Set to true for testing, false for production
   ```

### Getting Your Credentials

1. **Pi API Key**:
   - Visit the [Pi Developer Portal](https://developers.pi)
   - Create a new app or select your existing app
   - Copy the API Key from your app settings

2. **Merchant Wallet**:
   - Open your Pi wallet
   - Copy your wallet address
   - This is where donations will be sent

3. **Sandbox Mode**:
   - Use `true` during development and testing
   - Switch to `false` when deploying to production

## Development

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

## Building for Production

```bash
# Build the app
npm run build

# Preview the build
npm run preview
```

## Important Notes

- Always test payments in sandbox mode first
- Keep your API keys and wallet address private
- Never commit your `.env` file to version control