# ToutBot Prestige — Cloudflare Workers + D1

Portage de **ToutBot Prestige** sur Cloudflare Workers avec base de données **D1**.

## Fonctionnalités

- Authentification (inscription / connexion)
- Portefeuille Mobile Money (dépôts, retraits, soldes atomiques)
- Fil social + Shorts YouTube
- Abonnements payants aux créateurs
- Chat IA (Pollinations) avec recherche hybride
- Actu temps réel **sans clé API** :
  - DuckDuckGo Actu (Direct)
  - Google News RSS
- Messages privés utilisateur ↔ admin
- Panneau d’administration

## Fichiers

| Fichier        | Rôle                                      |
|----------------|-------------------------------------------|
| `worker.js`    | Application complète (Worker)             |
| `schema.sql`   | Schéma de la base D1                      |
| `wrangler.toml`| Configuration Cloudflare                  |
| `deploy.sh`    | Script de déploiement                     |

## Déploiement

### 1. Prérequis

```bash
npm install -g wrangler
wrangler login
