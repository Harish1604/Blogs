# 🔒 DeduVault: Our Journey into Decentralized Image Deduplication

*July 2025 • Project Log from the Edge of Cloud x Chain*

---

## 🚀 TL;DR

We built **DeduVault** — a decentralized image deduplication system that merges IPFS + Blockchain + Python into a sleek Streamlit UI. It flags duplicate images, stores hashes on-chain, and turns boring uploads into tamper-proof magic.

No central server. No repeats. No compromises. Just 🔐 integrity.

---

## 🧠 The Problem We Tackled

Cloud storage is cheap... until it's full of duplicates.

Imagine 1000s of people uploading the *same image* across platforms — wasting space, money, and compute. Centralized solutions can detect it, sure, but they can’t prove it. Worse, you’ve got **no audit trail** to trust.

So we asked:

> **What if you could detect duplicates, prove originality, and store data across the chain + cloud — transparently?**

---

## 🛠️ Tech Stack That Made It Happen

| Layer             | Tech Used                                                   |
|------------------|-------------------------------------------------------------|
| 🌐 **Frontend**     | Streamlit (Python)                                          |
| 🧠 **Backend**      | Python + Web3.py + JSON-based dedup DB                      |
| 🔗 **Blockchain**   | Solidity Smart Contract on Polygon Amoy (Mumbai earlier)    |
| 📦 **Storage**      | IPFS (via Pinata)                                           |
| 🧮 **Hashing**      | SHA-256 (for secure deduplication)                          |
| 🧪 **Testing**      | Remix IDE + Ankr RPC + Python API calls                     |

---

## 🔄 The Flow: How It Works

1. 🖼️ **User Uploads an Image**  
   ➤ We generate a **SHA-256 hash** of the file.

2. ⚙️ **Dedup Check**  
   ➤ That hash is checked **on-chain** using a Solidity contract.

3. 🚫 **Duplicate?**  
   ➤ If the hash exists, we block the upload and show a warning.

4. ✅ **New Image?**  
   ➤ We upload it to **IPFS via Pinata**, get the CID, and store the hash + CID on-chain.

5. 💻 **Display**  
   ➤ On click, the same image is rendered in a **3-column layout**, mimicking platforms like Amazon, Flipkart, and Meesho.

---

## 💥 Features That Hit Hard

- ✅ Blockchain-based hash registry  
- ✅ SHA-256 dedup engine  
- ✅ IPFS CID generation + storage  
- ✅ Streamlit UI with real-time feedback  
- ✅ JSON-based local cache (for dev preview)  
- ✅ CID-based image rendering across “fake” marketplaces

---

## 😵‍💫 Challenges We Slapped

- **Gas Fees** – Ran out of Sepolia ETH mid-test (classic)
- **IPFS Bugs** – CID mismatch due to wrong content-type headers
- **MetaMask Hell** – So we ditched it and went full Remix + Python
- **Smart Contract Integration** – Debugging Solidity with Python = pain
- **UI Edge Cases** – Handling browser drag-drop vs file select uploads

---

## 🧠 Lessons Learned

- Solidity gas costs teach you to *optimize everything*  
- Hashing is your best friend in any integrity-based system  
- Streamlit is 🔥 for building clean UIs fast  
- IPFS is cool but not perfect — **pinning is mandatory**
- On-chain + off-chain = 🔐 trust + 🧠 logic

---

## 🚧 What’s Cooking Next?

- 🔗 Ethereum Sepolia mainnet deployment (post faucet refill 💧)  
- 📊 Admin dashboard for viewing hash stats  
- 🧾 NFT-based proof of upload (optional)  
- 🧠 AI model to suggest “similar” images before storing  
- 📂 File type support beyond images (PDFs, Docs)

---

## 👨‍🚀 Our Dedup Dev Stack

```bash
- Python 3.11
- Streamlit
- Web3.py
- IPFS + Pinata SDK
- SHA-256 Hashlib
- Solidity + Remix IDE
- Ankr RPC for Polygon Amoy
