# URL Shortener

A sleek, dark-themed web app to instantly shorten URLs, generate stylish QR codes, and manage your link history—all with a beautiful, modern interface.

## ✨ Features
- **Instant Link Shortening:** Quickly trim long URLs with a single click.
- **Custom Aliases:** Personalize your short links with custom slugs.
- **QR Code Generation:** Create, download, and copy QR codes (with logo overlay) for any link.
- **Clipboard Actions:** Copy both short links and QR codes directly to your clipboard.
- **Recent History:** View and manage your 10 most recent shortened URLs.
- **Responsive Design:** Looks great on all devices.
- **Consistent UI:** Uses the Montserrat font and a unified dark color palette for a premium feel.

## 🚀 Getting Started
1. **Clone or Download:**
   - Download this repository as a ZIP or clone it using `git clone`.
2. **Open in Browser:**
   - Open `index.html` directly in your web browser.
3. **Shorten & Share:**
   - Paste your long URL, set a custom alias (optional), and click **Trim Link**.
   - Download or copy the generated QR code, and manage your recent links in the history section.

## 🌐 API Setup
To use this URL Shortener, you need your own RapidAPI credentials for the URL Shortener Service. This allows you to generate short links securely and independently.

### 1. Get Your RapidAPI Key
- Sign up or log in at [RapidAPI](https://rapidapi.com/).
- Subscribe to the [URL Shortener Service](https://rapidapi.com/BigLobster/api/url-shortener-service/) (or a similar one).
- Copy your API key (usually labeled `X-RapidAPI-Key`).

### 2. Create Your `config.js`
In the project root, create a file named `config.js` with the following content:

```js
const config = {
    RAPIDAPI_KEY: 'YOUR_RAPIDAPI_KEY', // Replace with your actual RapidAPI key
    RAPIDAPI_HOST: 'url-shortener-service.p.rapidapi.com' // Usually fixed for this service
};
```
- **Important:** This file is excluded from version control (see `.gitignore`). However, since it's loaded by the browser, your API key will be visible in browser dev tools during use.

### 3. Run the App
- For best results, use a local development server (e.g., VS Code's Live Server extension) to open `index.html`.
- You can also open `index.html` directly in your browser, but some features may work more reliably with a server.

## 🛠️ Tech Stack
- **Frontend:** HTML, CSS (with Montserrat font), JavaScript
- **QR Codes:** [qr-code-styling](https://github.com/kozakdenys/qr-code-styling)
- **Icons:** [Font Awesome](https://fontawesome.com/)

## 📄 License
This project is for educational and personal use. Please credit the original idea if you use or modify this project.

---

## 🙏 Credits
- Idea and inspiration: [unshreif](https://github.com/unshreif)
- QR code generation: [qr-code-styling](https://github.com/kozakdenys/qr-code-styling)
- Icons: [Font Awesome](https://fontawesome.com/)
- Font: [Montserrat](https://fonts.google.com/specimen/Montserrat)

> This theme and design were created by [shaswatacharya](https://github.com/shaswatacharya), inspired by the original work of [unshreif](https://github.com/unshreif). The goal was to build upon the original idea, adding my own touch and improvements to deliver a more refined and feature-rich version while giving full credit to the source of inspiration.
