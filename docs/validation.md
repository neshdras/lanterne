# Validation des routes

## Route /curiosities

code attendu : 200

Resultat: Affiche toutes les données de curiosities.json

![preuve validation route /curiosities](https://github.com/neshdras/lanterne/blob/main/docs/validation_img/curiosities.png)

## Route /curiosities?query

code attendu : 200

Resultat: Affiche toutes les données de curiosities.json selon les filtres imposé entre category, limit et query

![preuve validation route /curiosities?category&limit](https://github.com/neshdras/lanterne/blob/main/docs/validation_img/limite&category.png)

## Route /curiosities/:slug

code attendu : 200

Resultat: Affiche toutes les données d'une curiosité choisi, nommé par son slug

![preuve validation route /curiosities/:slug](https://github.com/neshdras/lanterne/blob/main/docs/validation_img/slug-tag.png)

## Route /health

code attendu : 200

Resultat: Affiche les information de l'API

![preuve validation route /health](https://github.com/neshdras/lanterne/blob/main/docs/validation_img/health.png)

## Route /curiosities/:falsecuriosity

code attendu : 404

Resultat: Retour une erreur pour donnée non trouvée

![preuve validation route /curiosities/:falseslug](https://github.com/neshdras/lanterne/blob/main/docs/validation_img/slugtag_falses.png)

## Route /falseroute

code attendu : 404

Resultat: Retour une erreur pour route non trouvée

![preuve validation route /:falseroute](https://github.com/neshdras/lanterne/blob/main/docs/validation_img/false_route.png)