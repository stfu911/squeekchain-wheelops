# SQUEEK RUN // Hamster-Powered Arcade, Stream Companion & SqueekFi Studio

Verified project for Squeekchain Genesis: https://squeekchain-wheelops.vercel.app / https://squeekops.abrdns.com

An interactive Proof-of-Hamster (PoH) arcade runner, dynamic NFT merge forge, and live telemetry OBS broadcast overlay built directly for the **Squeekchain** ecosystem.

---

## 🌟 Overview & Features

Unlike generic read-only dashboards, **Squeek Run** is an interactive, multi-dimensional Web3 application designed to engage the Squeekchain community across gaming, tokenomics, content creation, and telemetry:

1. **🐹 Squeektoshi Dash (Interactive Arcade Runner)**:
   - High-performance 60fps HTML5 Canvas game driven by **real hardware telemetry** from Squeektoshi's wheel on Ethereum Sepolia.
   - Connected live to `https://api.squeekchain.com/v1/status`: wheel speed, rim speed, and obstacle difficulty dynamically adjust based on whether the hamster is `SPINNING` or `IDLE`.
   - Procedural 8-bit sound effects synthesized dynamically via the Web Audio API (zero audio 404s).
   - "Zoomies" bonus multipliers when RPM > 120 and nap obstacles when Squeektoshi sleeps.

2. **🧪 10-Tier SqueekFi Merge Forge & Yield Calculator**:
   - Implements Squeekchain's exact integer tokenomics and staking equations from the protocol whitepaper:
     $$W = P + \frac{S \times (1 + P/1000)}{c}$$
   - Full 10-Tier Merge Pyramid simulator modeling cooldowns (0 to 49,000 blocks) and power scaling (+120% per merge).
   - Live SVG Generative Hamster Avatar Creator with customizable fur hues, goggles, ninja headbands, and crowns. Exportable as clean standalone SVG vector art.

3. **📺 OBS / Streamlabs Live Broadcast HUD (Stream Companion)**:
   - Instant 1-click toggle into a transparent, ultra-clean broadcast overlay for Twitch, Kick, and YouTube streamers.
   - Designed to sit alongside the official Squeekchain 24/7 hamster livestream with zero visual clutter.
   - Access via URL parameter: `https://squeekops.abrdns.com/?mode=overlay`.

4. **⚡ Web3 Sepolia Integration & "The Tester" Badge Ping**:
   - Native Web3 wallet connector (MetaMask, Rabby, Coinbase Wallet).
   - Built-in "Ping SQK" transaction button executing a safe, zero-gas `approve(self, 0)` on the official Sepolia SQK token contract (`0x5501e1fa81be1c3f49225fa7668da0245d07db60`), instantly qualifying the user for the coveted **The Tester** badge on Squeekchain Genesis!

---

## 🚀 Deployment Guide

### Deploying to Vercel (Recommended)

1. Deploy directly using the Vercel CLI:
   ```bash
   npx vercel deploy --prod
   ```
2. In the Vercel project dashboard under **Settings > Domains**, attach your custom domain (`squeekops.abrdns.com` or your own domain).

### Deploying to Cloudflare Pages / GitHub Pages

- Simply upload `index.html` to your repository or Cloudflare Pages project.
- Custom domain mapping will automatically serve the static bundle.

---

## 🔑 Squeekchain Genesis Verification Steps

To get your project approved for **The Buildooooor** badge on [Squeekchain Genesis Code Lane](https://squeekchain.com/genesis/code):

1. **Page Tag**: The `<meta name="squeekchain-verification" content="squeekops-genesis-verified">` is embedded in the `<head>` of `index.html`.
2. **README Line**: The first line of this README explicitly references the project URL.
3. **DNS TXT Record**: Add the verification token provided by the Squeekchain Genesis dashboard to your domain DNS provider (ClouDNS / Cloudflare / Namecheap):
   - **Type**: `TXT`
   - **Host**: `@` (or `squeekops`)
   - **Value**: The token string from Squeekchain (e.g. `squeekchain-verify=...`)
4. Return to [Squeekchain Genesis](https://squeekchain.com/genesis/code) and click **Verify Connection**.

---

## 📜 Verified Squeekchain Sepolia Contracts

| Contract | Address |
| :--- | :--- |
| **SqueekCore** | `0x980b4424c007caf7a1f3670b48c8eaef7ebc3d44` |
| **SQK Token** | `0x5501e1fa81be1c3f49225fa7668da0245d07db60` |
| **Mining Proxy** | `0xcd46990f8349057335289ef282c276204b6cdc62` |
| **Staking Proxy** | `0x4b67b739dfd832f4eac67a7aa3bc244fb74cea4f` |
