# Mega Bonus :skull:

On aurait pu l'appeler le _Mega Bonus de la mort_, mais on s'est contenté de l'appeler _Mega Bonus_ et d'ajouter un crâne à côté...

**Notre objectif**  
écrire une série de classes qui vont nous simplifier la vie pour créer des sites _responsives_

## Créons des classes utiles !

Créer un fichier vierge, que l'on va appeler `grid.css`.  
Dedans, nous allons coder une série de classe.

Définissons pour commencer les noms de tailles d'écran suivant :
* Extra-small (`xs`) : en-dessous de 600px
* Small (`sm`) : entre 600 et 900px
* Medium (`md`) : entre 900 et 1200px
* Large (`lg`) : au-dessus de 1200px

Pour ces 4 tailles, on va se créer des classes.  
Prêt ? C'est parti !

### Disparition

Il nous faut des classes permettant aux boites de disparaitre selon une taille d'écran.  
Par exemple : `<div class="box hidden-sm">` permet de faire disparaitre cette boite entre 600 et 900px.

Ecrire les classes pour les 4 tailles d'écran : `.hidden-xs`, `.hidden-sm`, `.hidden-md` et `.hidden-lg`.

### Des colonnes

Prenons comme postulat de découper la page en 12 colonnes.
On va s'écrire des classes permettant d'afficher de donner une largeur en colonnes à nos boites.

Par exemple : `<div class="box col-xs-6 col-sm-9">`
* En dessous de 600px, la boite prend 6 colonnes sur 12 (soit 50% de la page)
* **A partir de 600px** (et non seulement entre 600 et 900), la boite prend 9 colonnes sur 12 (soit 75% de la page)

Ecrire les classes `.col-{taille}-{colonnes}`.  
`.col-xs-1`, `.col-xs-2`, `.col-xs-3`, …, `.col-sm-1`, `.col-sm-2`, …, `.col-md-1`, `.col-md-2` …, `.col-lg-11`, `.col-lg-12`.

Oui, ça fait **48 classes**. Heureusement, le copier-coller existe !

### On pousse, on tire

Une boite peut désormais avoir une largeur exprimée en colonnes.
Sur le même principe, on va pouvoir bouger une boite d'un certain nombre de colonnes.

Par exemple : `<div class="box col-xs-push-2 col-sm-push-0 col-md-pull-3">`
* En dessous de 600px, la boite est décalée de 2 colonnes vers la droite
* A partir de 600px, la boite n'est plus décalée (elle est décalée de 0 colonnes)
* A partir de 900px, la boite est décalée de 3 colonnes vers la gauche

Ecrire les classes `.col-{taille}-{decalage}-{colonne}`.  
`.col-xs-push-0`, `.col-xs-push-1`, …, `.col-lg-pull-12`.

Ouais, là ça fait un paquet de classe !
**104 classes** pour être précis.
Novice en copier-coller s'abstenir.

## On remet ça ?

* Commenter ce que vous avez ajouté dans `style.css`, et ajouter `grid.css`.
* Refaire le challenge uniquement avec les classes qu'on vient de créer, en rajoutant des classes dans `index.html`.
