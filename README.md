# 📜 get-discord-token
A simple guide on how to easily retrieve your Discord token using the browser's developer tools.

> [!WARNING]
> Unauthorized use of a Discord token may violate Discord's Terms of Service and result in account suspension. Use this information responsibly.

---

## ❓ How to Retrieve Your Discord Token?

Cette méthode consiste à intercepter une requête réseau pour extraire l'en-tête d'autorisation contenant votre jeton.

### 1. Ouvrir Discord dans un navigateur
Connectez-vous à votre compte Discord via un navigateur web (Chrome, Firefox, Edge, etc.) sur [discord.com/app](https://discord.com/app).

### 2. Accéder aux Outils de Développement
- Appuyez sur `F12` (ou `Ctrl + Shift + I` sur Windows/Linux, `Cmd + Option + I` sur Mac).
- Cliquez sur l'onglet **Network** (Réseau) en haut de la fenêtre qui vient de s'ouvrir.



### 3. Filtrer et Trouver la Requête
- Dans la barre de recherche "Filter" de l'onglet Network, tapez `/api`.
- Si la liste est vide, rafraîchissez la page (`F5`) ou changez de salon (cliquez sur un autre serveur ou un ami).
- Sélectionnez l'une des requêtes qui apparaît dans la liste (par exemple `science`, `messages` ou `library`).

### 4. Extraire le Token
- Une fois la requête sélectionnée, allez dans la section **Headers** (En-têtes) à droite.
- Cherchez la ligne nommée **`authorization`** dans la catégorie "Request Headers".
- La valeur à côté de `authorization` est votre **Token Discord**. Copiez-la soigneusement.

---

> [!CAUTION]
> - **NE PARTAGEZ JAMAIS** votre token. Quiconque possède ce jeton a un accès total à votre compte (messages, serveurs, paramètres) sans avoir besoin de votre mot de passe ou de l'A2F.
> - Si vous pensez que votre token a été compromis, **changez immédiatement votre mot de passe Discord**. Cela réinitialisera automatiquement votre jeton.

**This guide is intended for learning and understanding how Discord works. Any malicious use is strictly prohibited.**
