# 📜 get-discord-token
A simple guide on how to easily retrieve your Discord token using the browser's developer tools.

> [!WARNING]
> Unauthorized use of a Discord token may violate Discord's Terms of Service and result in account suspension. Use this information responsibly.

---

## ❓ How to Retrieve Your Discord Token?

This method involves inspecting network requests to extract the authorization header containing your unique token.

### 1. Open Discord in a Browser
Log in to your Discord account via a web browser (Chrome, Firefox, Edge, etc.) at [discord.com/app](https://discord.com/app).

### 2. Open Developer Tools
- Press `F12` (or `Ctrl + Shift + I` on Windows/Linux, `Cmd + Option + I` on Mac).
- Click on the **Network** tab at the top of the developer panel.

### 3. Filter and Find the Request
- In the "Filter" search bar of the Network tab, type `/api`.
- If the list is empty, refresh the page (`F5`) or switch to a different server or DM.
- Select any of the requests that appear in the list (e.g., `science`, `messages`, or `library`).

### 4. Extract Your Token
- Once a request is selected, look at the **Headers** section on the right.
- Scroll down to the **Request Headers** category.
- Find the line named **`authorization`**.
- The value next to `authorization` is your **Discord Token**. Copy it carefully.

---

> [!CAUTION]
> - **NEVER SHARE** your token with anyone. Anyone with this token has full access to your account (messages, servers, settings) without needing your password or 2FA.
> - If you suspect your token has been compromised, **change your Discord password immediately**. This will automatically reset your token and invalidate the old one.

**This guide is intended for learning and understanding how Discord works. Any malicious use is strictly prohibited.**
