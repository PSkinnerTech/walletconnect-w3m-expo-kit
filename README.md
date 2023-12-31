# WalletConnect's Web3Modal Expo Starter Kit

This Starter Kit is designed for Expo ^49.0.0 with `expo-router`. It provides an easy-to-use foundation for integrating WalletConnect's `web3modal` into your Expo app.

## Features

- Expo ^49.0.0 setup with TypeScript.
- Routing with `expo-router`.
- WalletConnect's `web3modal` integration.
- Pre-configured for mainnet, polygon, and arbitrum chains.

## Prerequisites

- [Node.js](https://nodejs.org/)

## Notes:

-At this moment, this works cross platform from iOS and Android, but not web. This is actively being worked on so that an app can be built for all three platforms.

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

3. **Setup WalletConnect**:

   - Navigate to [WalletConnect Cloud](https://cloud.walletconnect.com).
   - Set up an account.
   - Start a new project.
   - Copy the project ID.
   - Open `/app/_layout.tsx` in your code editor.
   - Update the `const projectId` with the copied project ID.
   - Note: The metadata below can be updated later before you deploy your application.

4. **Start the Expo App**:

   ```bash
   npx expo start
   ```

5. **Run Simulation**:

   - You can run a simulation, but to best simulate the WalletConnect experience, you should run the app on a physical device by scanning the QR code with the Expo Go app.
   - If you do not have the Expo Go app, download it from the [App Store](https://apps.apple.com/us/app/expo-go/id982107779) or [Google Play](https://play.google.com/store/apps/details?id=host.exp.exponent&hl=en_US&gl=US).
   - If you don't have an Expo account, create one to run the app on a physical device.
   - Currently, do not attempt to run the app on the web, as Web3Modal v3 for react-native does not support desktop browser functionality.

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
