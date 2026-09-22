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
POur initialiser Vercel sur la machine

`npm i -g vercel`

## Etape 2 
Connexion 

`vercel login`
suivre les indication de vercel pour la connexion

## Etape 3 
Initialiser la variable LANTERNE_ENV 
`vercel --env LANTERNE_ENV=production`
