# Objets
## *person*
Tout être humain.
### propriétés
- `birth_year`
- `gender`
- `ethnicity` si disponible
- `profession` si disponible

## *execution*
Évènement exécution.
### propriétés
- `date`
- `method` : méthode léthale

## *geographical place*
Lieu.
### propriétés
- `type` : État, ville, etc.
- `long` : longitude
- `lat` : latitude

## *conviction*
Condamnation
## propriété
- `date`
- `reason`

# Relations

## *person* → *geographical place*
- Chaque personne est née à 1 endroit
- Chaque endroit peut avoir vu naitre 0-n personnes

## *person* → *execution*
- Chaque personne peut avoir subi 0-1 exécutions (pas sûr : quid des exécutions pas réussies ?)
- Chaque exécution peut avoir concerné 1-n personnes (pas sûr : y a-t-il eu des exécutions de groupe après 1976 ?) 

## *execution* → *geographical_place*
- Chaque exécution a eu lieu à 1 endroit
- Chaque endroit peut avoir accueilli 0-n exécutions

## *person* → *conviction*
- Chaque personne peut avoir eu 0-n condamnations
- Chaque condamnation concerne 1 personne (pas sûr)
