# 🟢 MINIMAL - Quick Start Web3 DevContainer

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&template_repository=theredguild/web3-devcontainer-minimal)
[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/theredguild/web3-devcontainer-minimal)

## 🚀 One-Click Deployment

This repository provides a ready-to-use Web3 development environment that you can launch instantly:

- **🚀 GitHub Codespaces**: Click the badge above or use the green "Code" button → "Create codespace"
- **🔧 Gitpod**: Click the Gitpod badge above for browser-based development
- **💻 Local VS Code**: Clone this repo and open with Dev Containers extension

## 🎯 Purpose
A minimal, beginner-friendly Web3 development environment focused on **ease of use** and **quick setup**. Perfect for learning, prototyping, and simple projects where security is not the primary concern.

## 🛡️ Security Level: **BASIC**

### Security Decisions & Rationale:

#### ✅ **What We Include (Minimal Security)**
- **Non-root user**: Uses `node` user instead of root
- **Standard permissions**: Normal file system access
- **Basic toolchain**: Only essential Web3 development tools
- **Standard networking**: Full internet access for package installs

#### ❌ **What We Don't Include (Simplified for Learning)**
- No advanced security hardening
- No capability dropping
- No filesystem restrictions
- No network limitations
- No custom seccomp profiles

### 🔧 **Technical Specifications**

| Component | Choice | Rationale |
|-----------|--------|-----------|
| **Base Image** | `mcr.microsoft.com/devcontainers/javascript-node:1-20-bullseye` | Official Microsoft devcontainer with Node.js 20, well-tested in Codespaces/Gitpod |
| **User** | `node` (non-root) | Basic security practice without complexity |
| **Tools** | Foundry, Hardhat, OpenZeppelin | Core Web3 development stack |
| **Extensions** | 4 essential extensions | Minimal VS Code setup for Solidity development |
| **Ports** | 3000, 8545 | Standard Web3 development ports |

### 🚀 **Compatibility**

✅ **GitHub Codespaces**: Fully compatible, uses official Microsoft base image  
✅ **Gitpod**: Fully compatible, standard devcontainer specification  
✅ **Local VS Code**: Works with Dev Containers extension  

### 📦 **Pre-installed Tools**

- **Solidity Compiler**: Latest via Foundry
- **Foundry**: `forge`, `cast`, `anvil` 
- **Hardhat**: Ethereum development environment
- **OpenZeppelin**: Secure smart contract library
- **Git**: Version control with GitHub CLI

### 🎨 **VS Code Extensions**

- `JuanBlanco.solidity` - Solidity language support
- `NomicFoundation.hardhat-solidity` - Hardhat integration
- `ms-vscode.vscode-json` - JSON editing
- `eamodio.gitlens` - Git visualization

### 🚀 **Quick Start**

1. **GitHub Codespaces**: Click "Code" → "Codespaces" → "Create codespace"
2. **Gitpod**: Prefix your repo URL with `https://gitpod.io/#`
3. **Local**: Open in VS Code with Dev Containers extension

### ⚠️ **Security Considerations**

**When to use**: 
- Learning Solidity and Web3 development
- Proof of concepts and prototypes
- Personal projects and experimentation
- Educational environments

**When NOT to use**:
- Production development
- Handling sensitive private keys
- Working with mainnet contracts
- Enterprise or team development
- Security-sensitive projects

### 🔄 **Upgrade Path**

When you outgrow this setup, consider upgrading to:
- **[SECURE](https://github.com/theredguild/web3-devcontainer-secure)** - Production development with security tools
- **[HARDENED](https://github.com/theredguild/web3-devcontainer-hardened)** - Enterprise-grade with compliance features
- **[AUDITOR](https://github.com/theredguild/web3-devcontainer-auditor)** - Read-only security analysis environment
- **[ISOLATED](https://github.com/theredguild/web3-devcontainer-isolated)** - Maximum security for malware analysis

📋 **[View All DevContainer Types](https://github.com/theredguild/web3-devcontainer-hub)** - Decision matrix and comparison

---

*This configuration prioritizes simplicity and ease of use over security. Perfect for getting started with Web3 development!*