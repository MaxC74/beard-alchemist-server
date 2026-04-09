# Beard Alchemist — Serveur API

## Déploiement sur Railway (gratuit)

### 1. Crée un compte
→ https://railway.app (connexion avec GitHub)

### 2. Nouveau projet
- Clique "New Project"
- Choisis "Deploy from GitHub repo"
- Connecte ce dossier (ou upload les fichiers)

### 3. Variable d'environnement
Dans Railway → ton projet → "Variables" :
```
ANTHROPIC_API_KEY = sk-ant-xxxxxxxxxxxxxxxx
```

### 4. Récupère l'URL
Railway te donne une URL du style :
```
https://beard-alchemist-server-production.up.railway.app
```

### 5. Mets à jour l'appli
Dans src/screens/AIAssistantScreen.js, remplace :
```js
const SERVER_URL = 'https://TON-URL.railway.app';
```

---

## Test local
```bash
npm install
ANTHROPIC_API_KEY=sk-ant-xxx node server.js
```

Puis teste :
```bash
curl http://localhost:3000/
```
