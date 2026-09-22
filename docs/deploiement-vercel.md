# Prérequis :
    - Compte vercel
    - Node.js installé sur la machine
    

# Arborescence

    ├── node_module
    |
    ├── docs/
    |    ├── deploiement-vercel.md
    |    ├── validation.md
    |    └── veille.md
    |
    ├── src/
    |    ├── data/
    |    |    └── curiosities.json
    |    └── index.js
    |
    ├── tests/
    |     |
    |     └── api.test.js
    |
    ├── .env
    ├── .env.exemple
    ├── .gitignore
    ├── package-lock.json
    ├── package.json
    ├── pnpm-lock.yaml
    ├── README.md
    └──vercel.json

# Point d'entrée Express
src/index.js

# Variable d'environnement 
ALLOWED_ORIGIN est le nom de domaine autorisant les requetes, il est configuré par Cors. Toute requete sera avorter si le nom de domaine n'est initialisé dans le cors.
LANTERNE_ENV est la valeur du projet, soit production soit preview

# Version de Node.js
version 24 or sup for Vercel

# Route de l'API principale

- GET : /curiosities → lire toutes les curiosités
- GET : /curiosities/slug-tag → lire les informations d'un curiosité
- GET : /curiosities?category=:category → lire les curiosités classé dans une catégorie choisi
- GET : /health → lide le status de l'API

# Deploiement

## Etape 1
npm i -g vercel