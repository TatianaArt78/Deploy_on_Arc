![Built with Foundry](https://img.shields.io/badge/Built%20with-Foundry-blue)
![Deployed on Arc Testnet](https://img.shields.io/badge/Deployed%20on-Arc%20Testnet-green)

## 🌐 Deployment Details

✅ Successfully deployed to **Arc Testnet**

- **Deployer:** `0x8E3A079D4e48d8aC485c669367Ee6d60E4bF2dA6`  
- **Contract Address:** `0xF44789647F8FE0a27487b26eb92E4f3E1334487C`  
- **Transaction Hash:** [`0xfe4da8f10c5cb4e39c29772ae8c73a68068a303cb478d95f113039568f166efc`](https://testnet.arcscan.app/)

---

## ⚙️ Automated Deployment via GitHub Actions

**Workflow file:** `.github/workflows/deploy.yml`

Deployment is triggered manually from **Actions → Run workflow**.

**The workflow does the following:**
- Installs Foundry  
- Compiles the smart contract  
- Deploys it to the Arc Testnet using your wallet’s private key and RPC URL stored in GitHub Secrets

---

## 🧪 How to Reproduce

1. Create a new GitHub repository  
2. Add your Solidity file under `src/`  
3. Create two GitHub secrets in **Settings → Secrets → Actions**:
   - `PRIVATE_KEY` → your wallet private key (must have test tokens)
   - `ARC_TESTNET_RPC_URL` → Arc Testnet RPC endpoint  
4. Add the workflow file: `.github/workflows/deploy.yml`  
5. Run it from the **Actions** tab

---

## 📖 Resources

- 🌐 [Arc Docs – Deploy on Arc](https://docs.arc.network/arc/tutorials/deploy-on-arc)  
- 💧 [Arc Faucet](https://faucet.circle.com/)  
- 🔍 [Arc Explorer](https://testnet.arcscan.app/)
