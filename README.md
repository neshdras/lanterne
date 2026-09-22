# Lanterne API

Lanterne est une API REST Express qui référence des curiosités locales : lieux discrets, détails architecturaux et petites histoires de quartier.

## Pré-requis

- Node.js 20 ou supérieur
- pnpm 11 ou npm compatible

## Installation et lancement local

```text
npm install
npm run check
npm run test
npm run start
```

L’API est disponible sur `http://localhost:3000`.

Lien Vercel de l'API : [Lanterne](https://lanterne-seven.vercel.app/)

## Routes principales

- [Lanterne - Toutes les curiosités](https://lanterne-seven.vercel.app/curiosities)
- [Lanterne - Toutes les curiosités filtré selon une categori avec une limite de 1](https://lanterne-seven.vercel.app/curiosities?category=mémoire&limit=1)
- [Lanterne - Une curiosité](https://lanterne-seven.vercel.app/curiosities/passage-bleu)
- [Lanterne - Voire les informations de l'API](https://lanterne-seven.vercel.app/health)

Le déploiement cible Vercel. Les variables d’environnement sont listées dans `.env.example`. Aucune donnée sensible ne doit être ajoutée au dépôt.
