---
layout: "default"
title: "Flows Auth: Svelte Authentication Library with WebAuthn Support"
description: "Svelte authentication library with WebAuthn support for whitelabel apps. Secure, mobile-optimized, and fully tested. Perfect for Flow app projects. 🚀🔒"
---
# Flows Auth: Svelte Authentication Library with WebAuthn Support

![Flows Auth](https://img.shields.io/badge/Flows%20Auth-Svelte%20Library-blue?style=for-the-badge&logo=svelte)

Welcome to the **Flows Auth** repository! This library provides robust authentication solutions tailored for Thepia Flow applications, with a focus on modern security practices, including WebAuthn and passkey support.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Contributing](#contributing)
- [License](#license)
- [Releases](#releases)

## Features

- **WebAuthn Support**: Leverage the latest standards in authentication.
- **Passkey Integration**: Simplify user access while enhancing security.
- **Svelte Framework**: Designed specifically for Svelte applications.
- **Typescript Compatibility**: Type-safe code for better maintainability.
- **Whitelabel Options**: Customize the library to fit your brand.
- **OAuth Support**: Easy integration with existing OAuth providers.
- **Lightweight and Fast**: Optimized for performance in modern web applications.

## Installation

To install the Flows Auth library, run the following command:

```bash
npm install flows-auth
```

Make sure to include the library in your Svelte project to start using its features.

## Usage

Here’s a basic example of how to implement Flows Auth in your Svelte application.

### Setting Up

First, import the library into your Svelte component:

```javascript
import { Auth } from 'flows-auth';
```

### Initializing Authentication

You can initialize the authentication process as follows:

```javascript
const auth = new Auth({
    // Your configuration options
    clientId: 'YOUR_CLIENT_ID',
    redirectUri: 'YOUR_REDIRECT_URI',
});
```

### Logging In

To log in a user, call the `login` method:

```javascript
auth.login()
    .then(response => {
        console.log('Login successful:', response);
    })
    .catch(error => {
        console.error('Login failed:', error);
    });
```

### Logging Out

Logging out is just as straightforward:

```javascript
auth.logout()
    .then(() => {
        console.log('Logout successful');
    })
    .catch(error => {
        console.error('Logout failed:', error);
    });
```

### Handling WebAuthn

For WebAuthn, you can utilize the built-in methods to manage user credentials:

```javascript
auth.registerWebAuthn()
    .then(credential => {
        console.log('WebAuthn registration successful:', credential);
    })
    .catch(error => {
        console.error('WebAuthn registration failed:', error);
    });
```

## API Reference

### Auth Class

- **constructor(options)**: Initializes the Auth instance with the given options.
- **login()**: Initiates the login process.
- **logout()**: Logs the user out of the application.
- **registerWebAuthn()**: Registers a new WebAuthn credential.

### Options

- **clientId**: The ID of your application.
- **redirectUri**: The URI to redirect after authentication.
- **scopes**: The scopes required for OAuth authentication.

## Contributing

We welcome contributions! To contribute to Flows Auth, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/YourFeature`).
6. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Releases

To download the latest version of Flows Auth, visit the [Releases section](https://github.com/Rudragiri-Gosai/flows-auth/releases). Make sure to execute the downloaded files as per the instructions provided.

For the latest updates, check the [Releases](https://github.com/Rudragiri-Gosai/flows-auth/releases) section frequently.

## Topics

- Authentication
- Flows
- Library
- OAuth
- Passkeys
- Svelte
- Thepia
- Typescript
- WebAuthn
- Whitelabel

## Support

For support, please open an issue in the GitHub repository. We aim to respond promptly to any questions or concerns.

## Acknowledgments

Thanks to the Svelte community for their contributions and support. This library builds on the great work done by others in the field of web authentication.

![Svelte](https://img.shields.io/badge/Svelte-Community-orange?style=for-the-badge&logo=svelte)

## Contact

For inquiries, you can reach out via the GitHub issues page or contact the repository owner directly.

---

By using Flows Auth, you can simplify the authentication process in your applications while ensuring a high level of security.