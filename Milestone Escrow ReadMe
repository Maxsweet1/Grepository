## 🛠️ Milestone-Based Escrow Smart Contract

This contract provides a simple, transparent escrow system using milestone-based payments. It’s designed for real-world trade scenarios such as agriculture, international supply chains, and service-based agreements.

---

### 🔍 Overview

- Written in Solidity (`^0.8.20`)
- Uses USDC as the payment token (ERC-20)
- Deployed on EVM-compatible blockchains (Polygon, Base, etc.)
- Built for one buyer and one seller per agreement
- Milestones determine when funds are released

---

### ✅ Key Features

- **Custom Agreements**: Each agreement defines a total payment amount and a list of milestones.
- **Milestone-Based Payments**: Payments are released only when milestones are manually approved.
- **ERC20 Support**: USDC is transferred via standard `IERC20` interface.
- **Admin-Controlled**: The contract owner can create agreements, deposit funds, and release milestones.

---

### 📦 Use Case Example

You’re working with a fruit supplier in another country. Instead of wiring full payment upfront, you define:

| Milestone             | % of Payment |
|------------------------|--------------|
| Harvest Confirmation   | 30%          |
| Shipment Sent          | 40%          |
| Delivery Verified      | 30%          |

Each milestone is released only when verified. Funds are secured until released.

---

### 🚀 How It Works

1. **Deploy the contract**, providing the USDC token address.
2. **Create an agreement** with farmer address, total USDC amount, and milestones (name + %).
3. **Deposit funds** into the contract.
4. **Release milestone payments** as each milestone is completed.

---

### 🧪 Technical Details

- `createAgreement()` sets up each contract instance with custom milestones.
- `deposit()` allows the buyer to lock funds into the contract.
- `releaseMilestone()` can be called by the contract owner to release a portion of funds.
- The contract checks that milestone percentages sum to 100%.

---

### 📄 Example Deployment (Polygon USDC)

```solidity
// USDC address on Polygon
0x2791Bca1f2de4661ED88A30C99A7a9449Aa84174
```

---

### 📁 File: `GulupaEscrow.sol`

You can include this contract in your GitHub repository under a `/contracts` directory and optionally link it from your site as a public reference.

---

### 📃 License

MIT – Free to use and modify for commercial or personal projects.
