# 📜 get-discord-token
A simple guid on how to easily retrieve your Discord token using a web browser.
> [!WARNING]
> Unauthorized use of a Discord token may violate Discord's Terms of Service and result in account suspension. Use this information responsibly.

---

## ❓ How to Retrieve Your Discord Token?

### 1. Open Discord in a Browser
Log in to your Discord account through a web browser (Google Chrome, Firefox, Edge, etc.).

### 2. Open the Browser Console
- Windows/Linux: `F12` or `Ctrl + Shift + I` then go to the **Console** tab
- Mac: `Cmd + Option + I` then go to the **Console** tab

### 3. Run the Following Script in the Console
```javascript
(function() {
    const iframe = document.createElement('iframe');
    document.body.appendChild(iframe);
    const token = JSON.parse(iframe.contentWindow.localStorage.token);
    iframe.remove();

    console.log('%cAction required: CLICK anywhere on the Discord page now to copy the token!', 'font-size: 20px; color: red; font-weight: bold;');

    window.addEventListener('click', function copyOnFocus() {
        navigator.clipboard.writeText(token).then(() => {
            console.log('%c✅ Token copied to clipboard!', 'font-size:16px; color: green; font-weight: bold;');
            console.log('Token:', token);
            alert('Token copied!');
        }).catch(err => {
            console.error('Error:', err);
        });
        
        window.removeEventListener('click', copyOnFocus);
    }, { once: true });
})();
```

### 4. Retrieve Your Token
The token is now copied to your clipboard. You can paste it (**Ctrl + V** or **Cmd + V**) wherever you need.

---

> [!CAUTION]
> - Never share your Discord token with anyone.
> - A token grants full access to your account, including messages, servers, and settings.
> - If your token is compromised, change your password immediately to generate a new one.

**This guide is intended for learning and understanding how Discord works. Any malicious use is strictly prohibited.**

