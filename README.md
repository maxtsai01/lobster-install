# 🦞 龍蝦安裝服務 Lobster Install Service

> **訂閱 → 準備 → 安裝 → 開始用**
> 30-60 分鐘，你的 AI 助手就上線

---

## 📋 安裝前你需要準備

### 1️⃣ 大腦 — Claude AI
- 透過 [PremLogin](https://premlogin.com/max) 購買 Claude MAX
- 折扣碼：`max`（95折）或 `max90`（90折）
- 比官方便宜 $20+

### 2️⃣ 設備 — 選一個
| 方案 | 說明 | 適合誰 |
|------|------|--------|
| 🖥️ 自己的電腦 | Mac 或 Windows 都行 | 想省錢、輕量使用 |
| ☁️ VPS 虛擬主機 | 24 小時不關機 | 認真跑自動化 |

### 3️⃣ 遠端連線工具 — Tailscale
- 下載：[tailscale.com/download](https://tailscale.com/download)
- 免費、零配置、安全加密
- 安裝後登入 → 把你的 Tailscale IP 給我們

---

## 🔧 安裝流程

### Step 1：下載必要軟體（你來，5 分鐘）
1. 安裝 [Tailscale](https://tailscale.com/download) 並登入
2. 把你的 Tailscale 機器名稱或 IP 告訴我們

### Step 2：遠端安裝（我們來，30-60 分鐘）
我們透過 Tailscale 連入你的電腦，幫你裝好：
- ✅ OpenClaw（龍蝦本體）
- ✅ Node.js 運行環境
- ✅ Claude AI 串接
- ✅ 你選的模組（1-2 個）
- ✅ 資安防護套件
- ✅ 測試確認一切正常

### Step 3：開始使用（你來）
- 跟你的龍蝦說話，它就開始工作
- 有問題隨時在 LINE@ 問

---

## 💰 方案與價格

| 方案 | 內容 | 價格 |
|------|------|------|
| 🅰️ 自助安裝 | SOP 文件 + LINE@ 客服 | $100 USD/月（訂閱費） |
| 🅱️ 遠端協助 | Tailscale 遠端幫裝 | $100 USD/月 + 安裝費 |
| 🅲️ VPS 全託管 | 幫選 VPS + 全部裝好 | $100 USD/月 + 安裝費 + VPS 月費 |

> ⚠️ 每日安裝名額有限，依購買順序排程

---

## 📱 模組一覽

訂閱後全部模組通用，建議先裝 1-2 個熟悉操作：

| 模組 | 功能 |
|------|------|
| 🎬 video-analyzer | AI 影片分析引擎 |
| 🎯 lobster-adspower | AdsPower 多帳號自動化 |
| 🛒 lobster-1shop | 1Shop 電商自動化 |
| 🤝 lobster-manus | AI 雙引擎協作 |
| 📱 fb-auto-register | FB 自動註冊 |
| 🐰 followbunny | FB 社團自動互動 |
| 🌈 rainbow-life | 彩虹人生人格測驗 |
| 🖼️ ai-image-studio | AI 圖片處理 |
| 💬 lobster-line-automation | LINE@ AI 自動化 |
| 🤖 agent-orchestrator | 多代理協作 |
| 🦞 lobster-ai-warbook | 龍蝦兵法手冊 |

---

## 🖥️ Mac 安裝 SOP

```bash
# 1. 安裝 Homebrew（如果沒有）
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 2. 安裝 Node.js
brew install node

# 3. 安裝 OpenClaw
npm install -g openclaw

# 4. 初始化
openclaw init

# 5. 設定 Claude API Token
openclaw models auth paste-token --provider anthropic

# 6. 啟動
openclaw gateway start
```

---

## 🪟 Windows 安裝 SOP

```powershell
# 1. 安裝 Node.js
# 下載：https://nodejs.org/ (LTS 版本)

# 2. 開 PowerShell（管理員）
npm install -g openclaw

# 3. 初始化
openclaw init

# 4. 設定 Claude API Token
openclaw models auth paste-token --provider anthropic

# 5. 啟動
openclaw gateway start

# 6. 設為 Windows 服務（開機自動啟動）
openclaw gateway install
```

---

## ☁️ VPS 安裝 SOP

```bash
# 推薦：Ubuntu 22.04+ VPS
# 供應商：Contabo / Hetzner / DigitalOcean（$10-20/月）

# 1. SSH 進入 VPS
ssh root@your-vps-ip

# 2. 安裝 Node.js
curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash -
sudo apt-get install -y nodejs

# 3. 安裝 Tailscale
curl -fsSL https://tailscale.com/install.sh | sh
sudo tailscale up

# 4. 安裝 OpenClaw
npm install -g openclaw
openclaw init

# 5. 設定 Claude API
openclaw models auth paste-token --provider anthropic

# 6. 背景運行
openclaw gateway start
# 或用 pm2：
npm install -g pm2
pm2 start "openclaw gateway start" --name lobster
pm2 save
pm2 startup
```

---

## 🔒 資安套件（安裝時一併處理）

- Tailscale（加密 VPN 通道）
- 防火牆設定（只開必要 port）
- SSH Key 認證（VPS 專用）
- 自動更新設定

---

## 📬 聯絡

- 📸 IG: [@10000allison](https://www.instagram.com/10000allison/)
- 💬 LINE@: 加好友開始訂閱

---

*Created by Allison · CTMaxs · 🦞 龍蝦模組商店*

---

## 🦞 龍蝦模組商店 Lobster Store

**💎 $100 USD/月 — 全部模組通用，訂閱即開通**

> 📸 私訊 [@10000allison](https://www.instagram.com/10000allison/) 訂閱 → 付款 → 全部模組即刻開通
