# Le jeu des boîtes

De quoi travailler le responsive design :smiley:

## Instructions

* Les boîtes doivent être placées les unes sous les autres (sur 4 lignes).

![xs](images/xs.png)

* à partir de 600px de large :
  + les boîtes doivent être affichées sur deux lignes, avec deux boites par ligne (2 colonnes par ligne).
  + la boîte noire et la boîte verte doivent échanger leurs places.

![sm](images/sm.png)

* à partir de 900px de large :
  + la boîte noire doit disparaître
  + les autres boîtes doivent se placer à côté les unes des autres (3 colonnes sur une ligne).

![md](images/md.png)

* à partir de 1200px de large :
  + la boîte noire doit apparaitre à nouveau
  + les 4 boîtes sont dorénavent toutes à côté les unes des autres (4 colonnes sur une ligne).

![lg](images/lg.png)


## Pour info

Vous verrez que dans le `index.html`, il y a une petite nouveauté :
```html
<meta name="viewport" content="width=device-width, initial-scale=1">
```

Il s'agit d'une balise permettant de définir le niveau de zoom initial sur mobile.  
Pour en savoir plus, allez donc lire la fiche récap [Responsive Web Design](https://kourou.oclock.io/ressources/fiche-recap/rwd/) !


## Bonus

<details><summary>Tu es sûr(e) de vouloir faire le bonus alors que demain, c'est un parcours sur toutes les notions vues durant cette première saison ?</summary>

A priori, oui.  
Tu peux trouver le [bonus ici](bonus.md)

</details>
