# WalletConnect's Web3Modal Expo Starter Kit

This Starter Kit is designed for Expo ^49.0.0 with `expo-router`. It provides an easy-to-use foundation for integrating WalletConnect's `web3modal` into your Expo app.

## Features

- Expo ^49.0.0 setup with TypeScript.
- Routing with `expo-router`.
- WalletConnect's `web3modal` integration.
- Pre-configured for mainnet, polygon, and arbitrum chains.

## Prerequisites

- [Node.js](https://nodejs.org/)

## Getting Started

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/PSkinnerTech/walletconnect-w3m-expo-kit.git
   cd walletconnect-w3m-expo-kit
   ```

2. **Install Dependencies**:

   ```bash
   yarn install
   ```

3. **Start the Expo App**:

   ```bash
   npx expo start
   ```

4. **Run Simulation**:
   You can run simulation, but to best simulate the WalletConnect experience, you should run the app on a physical device by scanning the QR code with the Expo Go app.

### Update Project Metadata

In the `/app/_layout.tsx` file, you can update the `metadata` object to reflect your project's details:

```typescript
const metadata = {
  name: "Your Project Name",
  description: "Your Project Description",
  url: "Your Project URL",
  icons: ["Your Project Icon URL"],
  redirect: {
    native: "YourNativeRedirectURL",
    universal: "YourUniversalRedirectURL",
  },
};
```

### Add More Chains

If you wish to add more chains, update the `chains` array in `/app/_layout.tsx`.

## Troubleshooting

If you encounter any issues:

- Ensure all dependencies are correctly installed.
- Check the console for any errors and address them.
- Refer to the official [WalletConnect documentation](https://docs.walletconnect.com/web3modal/react-native/about) for more details on `web3modal`.

## Contributing

We welcome contributions! If you find a bug or have suggestions, please open an issue. If you'd like to contribute code, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License.

---

Feel free to modify or expand upon this documentation as needed. Let me know if you need any additional sections or details!
