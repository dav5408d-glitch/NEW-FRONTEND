# RIFT Frontend - Vercel Deployment

## Déploiement sur Vercel

1. Importez ce repo sur Vercel : https://vercel.com
2. Le déploiement se fera automatiquement.

## Configuration de l'API

Modifiez `config.js` pour pointer vers votre backend déployé :

```javascript
window.RIFT_CONFIG = {
  API_BASE_URL: 'https://votre-backend.vercel.app', // URL de votre backend
  OLLAMA_URL: 'http://localhost:11434' // Pour développement local
};
```

## Backend

Le backend est dans un repo séparé. Créez un repo `NEW-BACKEND` et poussez le contenu de `vercel-project/` pour déployer l'API.

## Développement local

Pour tester localement :
- Changez `API_BASE_URL` dans `config.js` vers `http://localhost:3000` ou votre URL locale.
- Lancez le backend avec `npm run dev` dans le dossier backend.