# 🚀 AEllina Agent: The Ultimate Universal MCP Gateway

**AEllina Agent** is a premium, all-in-one Windows desktop environment designed to empower AI Agents (Claude, Perplexity, etc.) with local system capabilities. It’s not just a connector; it’s a full-fledged **Command Center** for your AI agents, featuring a high-performance UI, secure tunneling, and stateful terminal sessions.


---

## 🔥 Full Feature Suite

### 🖥️ 1. Premium Desktop IDE
*   **Built-in File Explorer**: Manage your project structure directly within the app.
*   **Modern Code Editor**: Syntax-highlighted editor to view and edit files on the fly.
*   **Live Terminal**: A native terminal to see exactly what's happening.
*   **Command Activity Panel**: Watch AI-driven commands stream output in real-time, character by character.
*   **Customizable Aesthetics**: Switch between professional themes and scale font sizes for the editor, explorer, and terminal.

### 🐚 2. Stateful PowerShell Engine
*   **Persistent Sessions**: Unlike standard MCP servers, AEllina keeps PowerShell sessions alive. Environment variables, function definitions, and directory changes persist across multiple AI interactions.
*   **Background Jobs**: AI can start long-running tasks (like builds or servers) in the background while continuing with other work.
*   **Smart Output Handling**: Automatically trims massive logs while preserving head/tail info and extracting critical error snippets.

### 🛡️ 3. Industrial-Grade Security
*   **Human-in-the-Loop**: Every new connection request triggers a **Device Approval Popup**. No platform gets access without your click.
*   **Hybrid Routing**: Simultaneously supports Local access (Claude Desktop) and Public access (Perplexity) with zero-downtime switching.
*   **OAuth 2.0 Gateway**: Implements full Dynamic Client Registration (MCP Spec Nov 2025). Securely manage tokens and revoke any device instantly from the settings.

### 🌍 4. One-Click Connectivity
*   **Claude Desktop Sync**: Automatic detection and configuration of Claude's config files.
*   **Built-in Tunneling**: Seamless integration with **Ngrok** and **Cloudflare** to make your local MCP server accessible globally.

---

## 🛠️ Prerequisites (For Remote/Cloud AI)

### 🔌 1. Ngrok (Integrated)
1.  Download Ngrok: [ngrok.com/download](https://ngrok.com/download)
2.  Copy your **Auth Token** from: [dashboard.ngrok.com](https://dashboard.ngrok.com/get-started/your-authtoken)
3.  **No terminal needed**: Just paste the token in **AEllina UI > Settings > Tunnel** and click **Start**.

### ☁️ 2. Cloudflare (Stable)
Install via PowerShell (Run as Administrator):
```powershell
winget install Cloudflare.cloudflared
```
*Enable it instantly from the AEllina dashboard once installed.*

---

## 🚀 Getting Started

1.  **Install**: Download and run `AEllinaAgentSetup.exe` from the [Releases](https://github.com/masterkalii7/AEllinaAgent/releases/tag/v1.0.0) page.
2.  **Open Workspace**: Click "Open Folder" in the AEllina UI to set the root directory for your AI agent.
3.  **Local Use**: Simply restart **Claude Desktop**. AEllina automatically injects the tools.
4.  **Remote Use (Perplexity/Web)**:
    *   Start a tunnel (Ngrok/Cloudflare) in the app.
    *   Copy the `HTTPS` URL.
    *   Add it to your AI platform's MCP settings.
    *   Click **Approve** on the popup when the AI tries to connect.

---

## 🛠️ Included AI Toolsets

AEllina Agent exposes a powerful set of tools to your AI:
*   **Powershell_command**: Full access to Windows PowerShell (Stateful).
*   **Filesystem**: Read, write, list, and search files in your workspace.
*   **Core Tools**: System health, workspace info, and process management.
*   **Time Tools**: Timezone-aware date and time operations.

---

## 🔒 Security & Privacy

*   **Total Control**: You can approve or reject every single connection request.
*   **Session Management**: See exactly what the AI is doing in real-time through the "Activity" panel.
*   **Revocation System**: You have the master switch. Disconnect any platform or client at any time from the Security panel.
*   **Privacy**: Your local data is only shared with the AI model you choose to interact with.

---

## 📦 Technical Specs

*   **Runtime**: Python 3.10+ (Optimized & Compiled via Nuitka).
*   **UI Framework**: PyQt6.
*   **Server Engine**: Starlette & Uvicorn.
*   **Packaging**: Standalone EXE with NSIS Installer.

---

## 🤝 Support

AEllina Agent is a passion project by **masterkalii7**. If it helps your workflow, please consider giving it a ⭐️ on GitHub!

**Crafted with ❤️ for the AI community.**
