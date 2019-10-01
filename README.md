# Code créatif Module 01

## objectif
Réaliser à l'aide du langage Processing les exercices suivants.
Un exercice est soit raté, soit réussit, sauf indication contraire.
Chaque exercice rapporte des points, pour valider un module il faut obternir au moins 60% des points de l'ensemble du modules.
Dés que la norme n'est pas respectée, l'exercice est considéré comme raté.

L'ensemble des exercices sont à renvoyer par mail au correcteur en respectant l'arborescence et le nommage des dossiers, sous-dossiers et nom de fichiers. Si l'arborescence n'est pas respectée l'exercice ou le module ne seront pas corrigés et considérés comme ratés.
```
dossier : nom prénom
sous-dossier : module
sous-dossier : exercice
fichier : nom.pde
```

>exemple
Maurice Dupont/m00/m00_ex_00_truc/m00_ex_00_truc.pde

contraintes : 
respecter la norme https://github.com/StanLepunK/The_way_of_creative_code/blob/master/norme_voie_du_code.md


## m01_ex00_ellipse
```
sketch : m01_ex00_ellipse.pde
xp : 5
intitulé :
Dans une fenêtre de 640 par 480.
Faire apparaitre un cercle qui suit le position de la souris.
```
```
primitive : 
globale : 
operateur : 
methodes primaire : setup(), draw()
methodes secondaire : size(), ellipse()
condition :
itération :
```
## m01_ex01_background
```
sketch : m01_ex01_background.pde
xp : 5
intitulé :
Dans une fenêtre de 640 par 480.
Faire apparaitre un cercle qui suit le position de la souris et laisse une trace permanente derrière lui.
Quand on clique avec souris toutes trace diparait.
Une couleur pour l'arrière plan et une couleur pour le cercle, pas de contour.
```
```
primitive : 
globale : mousePressed
operateur : 
methodes primaire : setup(), draw()
methodes secondaire : size(), ellipse(), background()
condition :
itération :
```
## m01_ex02_couche_alpha
```
sketch : m01_ex02_couche_alpha.pde
xp : 5
intitulé :
Dans une fenêtre de 640 par 480.
Faire apparaitre un cercle qui suit le position de la souris et qui laisse une trace dérrière lui qui s'éfface petit à petit.
Une couleur pour l'arrière plan et une couleur pour le cercle, pas de contour.
```
```
primitive : 
globale : mousePressed
operateur : 
methodes primaire : setup(), draw()
methodes secondaire : size(), ellipse(), background(), noStroke(), fill(), rect()
condition :
itération :
```
## m01_ex03_evolution
```
sketch : m01_ex03_evolution.pde
xp : 10
intitulé : 
Dans une fenêtre de 640 par 480.
Faire apparaitre un cercle qui croit et décroit de façon régulière et qui suit le position de la souris.
Une couleur pour l'arrière plan et une couleur pour le cercle, pas de contour.
```
```
primitive : int, float
globale : frameCount, mouseX, mouseY
operateur : * + -
methodes primaire : setup(), draw()
methodes secondaire : size(), abs(), sin(), cos(), background(), noStroke(), fill(), ellipse()
condition :
itération :
```
## m01_ex04_detection_1
```
sketch : m01_ex04_detection_1.pde
xp : 10
intitulé : 
Dans une fenêtre de 640 par 480.
A l'intérieur un rectangle sera placé au centre avec une marge de 50 pixels autour.
Quand la souris passeras sur le rectangle celui-ci changera de couleur.
Un couleur pour la marge et deux couleurs pour les différents états du rectangle, pas de contour.
```
```
primitive : int
globale : mouseX, width, height
operateur : = > / - *
methodes primaire : setup(), draw()
methodes secondaire : size(), background(), noStroke(), fill(), rect()
condition : if, else
itération :
```
## m01_ex05_detection_2
```
sketch : m01_ex05_detection_2.pde
xp : 10
intitulé : 
Dans une fenêtre de 640 par 480.
A l'intérieur un rectangle sera placé au centre avec une marge de 50 pixels autour.
Quand la souris sera dans la partie gauche de la fenêtre le rectangle sera d'une couleur, quand la souris sera dans l'autre le rectangle sera d'une autre couleur.
Un couleur pour la marge et deux couleurs pour les différents états du rectangle, pas de contour.
```
```
primitive : int
globale : mouseX, mouseY, idth, height
operateur : = > < && - *
methodes primaire : setup(), draw()
methodes secondaire : size(), background(), noStroke(), fill(), rect()
condition : if, else
itération :
```
## m01_ex06_mvt_1
```
sketch : m01_ex06_mvt_1.pde
xp : 5
intitulé : 
Dans une fenêtre de 640 par 480. 
Créer un cercle de couleur qui se déplace de gauche à droite en descendant et sans laisser de trace.
L'arrière plan est d'une couleur et le cercle d'une autre, pas de contour.
```
```
primitive : int, float
globale : 10
operateur : = + >
methodes primaire : setup(), draw()
methodes secondaire : size(), background(), noStroke(), fill(), ellipse()
condition : if
itération :
```
## m01_ex07_mvt_2
```
sketch : m01_ex07_mvt_2.pde
xp : 10
intitulé : 
Dans une fenêtre de 640 par 480.
Créer un cercle de couleur qui se déplace et rebondit sur les paroies dés qu'un des côtés de celui-ci est en contact avec une des paroies de la fenêtre.
L'arrière plan est d'une couleur et le cercle d'une autre, pas de contour.
```
```
primitive : int, float
globale : width, height
operateurs : = + > < - * ||
methodes primaire : setup(), draw()
methodes secondaire : size(), background(), fill(), ellipse()
condition : if
itération :
```
## m01_ex08_extraball
```
sketch : m01_ex08_extraball.pde
xp : 30
intitulé : 
Dans une fenêtre de 640 par 480.
Créer un cercle de couleur qui se déplace et rebondit sur les paroies. 
Le cercle change de couleur quand la souris passe dessus. 
Le cercle peut être attrapé avec la souris pour être déplacé et si c'est le cas doit changer de couleur.
Il y a donc trois couleurs de cercle et une pour l'arrière plan. 
Le cercle doit grossir et rétrécir de façon régulière.
Si le clavier est présser l'arrière plan persiste pendant quelques secondes.
Si la souris est pressée l'arrière plan passe au noir.
L'exercice peut-être partielement réussit.
```
```
primitive : int, float
globale : width, height, mouseX, mouseY, mousePressed, keyPressed
operateurs : = + > < - * || &&
methodes primaire : setup(), draw()
methodes secondaire : size(), background(), fill(), ellipse(), stroke(), noStroke(), rect(), abs(), sin(), cos()
condition : if, else
itération :
```


