# 🎓 EduFi Learn-to-Earn

A decentralized education rewards system built on the **Cardano blockchain**.  
EduFi allows students to **learn, track progress, and earn ADA** for completing lessons verified on-chain.  
All progress and rewards are stored in a **Plutus V2 smart contract**—no intermediaries, no off-chain trust.

---

## 🌐 Live Demo
https://edufidapps.vercel.app/

---

## ✨ Features
- 🧩 **Enroll** directly using a Cardano wallet (Lace)
- 📚 **Track progress** stored on-chain as inline datums  
- 💰 **Earn ADA** automatically after completing all lessons  
- 🔒 **Plutus V2 validator** ensures secure state transitions  
- ⚡ **Lucid SDK** handles blockchain transactions in-browser  
- 🌍 100 % decentralized, transparent, and self-auditable  

---

## 🛠️ Tech Stack
- **Cardano Preprod Testnet**
- **Lucid Cardano SDK**
- **Plutus V2 Smart Contracts**
- **Blockfrost API**
- **Lace Wallet (CIP-30)**  
- **HTML + CSS + JavaScript Frontend**

---

## 📋 Requirements
- Lace Wallet browser extension  
- Preprod testnet ADA (from faucet)  
- Modern Chromium-based browser  
- A deployed EduFi script address

---

## 🚀 How to Use
1. **Connect** your Lace wallet  
2. **Enroll** with your wallet (optional stake amount)  
3. **Complete** lessons as you study  
4. **Claim** all rewards once every lesson is finished  

Transactions are fully validated by the EduFi Plutus V2 script and visible on Cardano explorers.

---

## 🧠 Smart Contract Overview
- **Network:** Cardano Preprod Testnet  
- **Validator Type:** Plutus V2  
- **Reward Logic:** `totalReward = totalLessons × rewardPerLesson`  
- **State Model:** Inline Datum (UTXO based)  
- **Script Address:** Generated in the dApp after wallet connection  

---

## 💡 Core Actions
| Action | Redeemer Index | Description |
|--------|----------------|-------------|
| **Enroll** | `Constr(0)` | Register a new student datum |
| **CompleteLesson** | `Constr(1)` | Increment `lessonsDone` count |
| **ClaimAll** | `Constr(2)` | Withdraw stake + rewards |

---

## 🔗 Resources
- [Cardano Preprod Faucet](https://docs.cardano.org/cardano-testnet/tools/faucet/)
- [Preprod Explorer](https://preprod.cardanoscan.io/)
- [Lace Wallet Official Site](https://www.lace.io/)
- [Lucid Cardano SDK Docs](https://lucid.spacebudz.io/)
- [Blockfrost API Docs](https://blockfrost.io/)

---

## 🧪 Testing Checklist
✅ Wallet connection works correctly  
✅ Student enrollment creates on-chain UTXO  
✅ Lesson completions update datum  
✅ Rewards can only be claimed after full completion  
✅ Transactions visible via Blockfrost Explorer  

---

## 📜 License
MIT License © 2026 EduFi Developers  

---

### 👨‍💻 Author
**Teslim Lyon**  
*Built with Lucid + Plutus V2 on Cardano Preprod Testnet*
