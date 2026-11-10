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
- Chaque personne peut avoir subi 0-1 exécution
- Chaque exécution concerne 1 personne (à priori)

## *execution* → *geographical_place*
- Chaque exécution a eu lieu à 1 endroit
- Chaque endroit peut avoir accueilli 0-n exécutions

## *person* → *conviction*
- Chaque personne peut avoir eu 0-n condamnations
- Chaque condamnation concerne 1 personne (à priori)

## *conviction* → *execution*
- Chaque condamnation peut mener à 0-1 exécution
- Chaque exécution peut être causée par 1 condamnation (à priori)

