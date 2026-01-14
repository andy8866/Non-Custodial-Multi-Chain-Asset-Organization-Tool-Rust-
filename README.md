# Non-Custodial Multi-Chain Asset Organization  
非托管多链资产整理（Rust 实现）

---

## Overview

**Non-Custodial Multi-Chain Asset Organization** is a **local-first, non-custodial blockchain asset management utility** written in **Rust**.

runs entirely in the **user’s local environment** and helps users **organize and consolidate on-chain assets** distributed across multiple addresses and multiple blockchain networks.

> ⚠️ This project is a **pure technical utility**.  
> It does **not** provide custody, payment, clearing, escrow, or fund management services.

---

## 项目概述

**非托管多链资产整理** 是一款基于 **Rust** 开发的 **本地运行、非托管** 的区块链资产整理。

运行在**用户自己的本地环境**中，用于帮助用户整理、归并分散在多个地址、多个区块链网络上的链上资产。

> ⚠️ 本项目仅为**技术工具软件**，  
> 不提供任何形式的资金托管、支付、清算或资金管理服务。

---

## Key Principles | 设计原则

### 🔐 Non-Custodial / 非托管

- Do not store private keys or mnemonic phrases
- No backend services, no cloud storage
- All transactions are **signed locally**

- 不保存 私钥 / 助记词 
- 不依赖服务器、不上传数据
- 所有交易均由用户本地签名

---

### 🧑‍💻 User-Controlled Execution / 用户完全控制

- Users explicitly provide:
  - Mnemonic phrase or private keys
  - Source addresses
  - Target addresses
  - Blockchain networks
- The tool only executes **user-confirmed instructions**

- 用户主动输入助记词或私钥
- 用户明确指定源地址与目标地址
- 工具仅按用户确认的指令执行，不具备自主决策能力

---

### 🛠 Technical Utility Only / 纯技术工具定位

- No custody
- No escrow
- No fund pooling
- No merchant system

- 不托管资产  
- 不提供代收代付  
- 不参与资金流转  
- 不提供商户或账户体系  

---

## Features | 核心功能

### 🌐 Multi-Chain Support | 多链支持

Supported networks include:

- Arbitrum  (Layer 2)
- TRON / TRC20

---

### 📦 Asset Organization | 资产整理

- Scan balances across multiple addresses
- Support HD wallets (multiple derived addresses)
- Consolidate assets into user-defined target addresses

- 扫描多个地址的链上资产
- 支持助记词派生的多个地址
- 将分散资产整理到指定地址

---

### ⛽ Fee & Resource Detection | 手续费检测

- Detect ETH / TRX balance availability
- Warn when gas or energy is insufficient
- Prevent failed transactions

- 检测手续费余额
- 提示补充 ETH / TRX
- 避免因手续费不足导致失败交易

---

### 🧾 Transparent Execution | 透明执行流程

- Read-only RPC for balance scanning
- Local transaction construction
- Local signing & broadcasting
- Full transaction hash visibility

---

## How It Works | 工作流程

1. User runs the tool locally  
2. Inputs mnemonic phrase or private keys (local only)  
3. Tool derives and scans addresses  
4. Fetches on-chain balances via RPC  
5. User confirms the organization plan  
6. Transactions are signed locally  
7. Transactions are broadcast to the blockchain  
8. Results are displayed to the user  

---

1. 用户在本地运行工具  
2. 输入助记词或私钥（仅本地使用）  
3. 工具派生并扫描地址  
4. 查询链上资产余额  
5. 用户确认整理方案  
6. 本地签名交易  
7. 广播交易到区块链  
8. 展示交易结果  

---

## Security Considerations | 安全说明

- ❌ No private key storage  
- ❌ No mnemonic backup  
- ❌ No remote execution  
- ✅ User-controlled signing  
- ✅ Transparent transaction flow  

---

## Legal & Compliance Disclaimer  
## 法律与合规声明（重要）

This software is a **self-hosted technical utility**.

- It does **not** custody user assets
- It does **not** initiate transactions without user authorization
- It does **not** provide financial or payment services

Users are solely responsible for:
- Key management
- Asset security
- Compliance with local regulations

---

本软件为**用户自部署的技术工具**：

- 不托管用户资产  
- 不在用户授权之外发起交易  
- 不构成金融服务或支付服务  

用户需自行承担：
- 私钥管理责任  
- 资产安全责任  
- 所在司法辖区的合规责任  

---

## Project Status | 项目状态

- Current stage: **Active development**
- Focus: Security, correctness, extensibility

---

## License

Specify license here (Commercial)
