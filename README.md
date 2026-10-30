# WheelOps // Squeekchain Consensus Terminal

Physical Proof-of-Hamster (PoH) node telemetry monitor and block validator built specifically for the Squeekchain ecosystem.

## Overview
WheelOps provides an interactive interface to monitor physical hamster wheel consensus metrics, calculate caloric-to-hash ratios, and inspect block propagation across the Squeekchain gossip mesh.

### Core Features
- **Physical Proof-of-Hamster Engine**: Interactive 60fps wheel simulation with inertia physics, caloric burn monitoring, and RPM hashing telemetry.
- **Cryptographic Block Packaging**: Real SHA-256 block hashing via Web Crypto API with dynamic wheel nonce generation.
- **Web3 Wallet Verification**: Injected EIP-1193 connector for wallet authentication.
- **Synthesized Audio Telemetry**: Procedural Web Audio API sound for wheel bearings and block mint alerts (zero asset dependencies).
- **Squeekchain Genesis Domain Proof Helper**: Integrated inspection modal for Squeekchain DNS TXT validation records.

---

## 1-Minute Deployment Guide

### Option 1: Deploy to Vercel (Easiest)
1. Push this folder to GitHub or run with Vercel CLI:
   ```bash
   npx vercel deploy --prod
   ```
2. In Vercel Project Settings -> **Domains**, assign your custom domain (e.g. `squeek.yourdomain.com` or `yourdomain.com`).

### Option 2: Deploy to Cloudflare Pages / GitHub Pages
- Simply upload `index.html` to Cloudflare Pages or GitHub Pages repository.
- Attach your custom domain in the dashboard settings.

---

## Squeekchain Genesis Quest Verification
1. Open the project submission form in Squeekchain Genesis:
   `https://squeekchain.com/genesis/u4fyts6q`
2. Enter your project URL: `https://yourdomain.com`
3. Squeekchain will give you a specific DNS TXT record (e.g. `squeekchain-verify=...`).
4. In your DNS provider (Cloudflare, Namecheap, GoDaddy):
   - **Type**: `TXT`
   - **Name**: `@` (or subdomain `squeek`)
   - **Content / Value**: The token from Squeekchain
5. Click **Verify Connection** on Squeekchain.
6. The Squeekchain team will inspect the live terminal and approve your Genesis Badge.

