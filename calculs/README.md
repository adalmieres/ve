# Dimensionnement grossier

Conditions considérés :
- sol plat
- vent nul
- résistance au roulement négligeable
- condition normal de température et de pression
- densité de l'air = 1.184 (sans unité)
- Cx = 1,2 (celui d'Usain Bolt)
- maitre couple = 0,56m² (source http://cyclurba.fr/velo/666/Cx-SCx-Watts-puissance-vitesse-rendement-aerodynamique.html)
- rendement global = 78%

## Puissance mini

### Approche par étude des forces

Le moteur doit produire une force de traction égale à la trainé aérodynamique (calcul dans le fichier ods)

Le calcul donne une puissance mini de __3750W__ en sortie du moteur. Soit __2925W__ à la roue.

### Approche par l'accélération

A partir de la puissance à la roue, nous en déduisons le temps d'accélération mini : __6,46 secondes__

## Dimensionnement des batteries

Pour une autonomie de __70km__ il faut donc en théorie __3750Wh__ d'énergie. En prenant des batteries de 48V cela donne une capacité totale de __78Ah__.
Soit __19kg__ de batterie LiPo en supposant une densité massique de 200Wh/kg.

Autre approche possible : partir de l'espace disponible et en déduire la quantité embarquable.

### Capacité embarquable

Supposons l'emplois de module lithium 18650 (cylindre d'un diamètre de 18,3mm) disposé en pavage carré sur la surface de l'intérieur du cadre.
Le cadre est approximé à un triangle de base 450mm et de hauteur 380mm.
La surface est donc de __85500mm²__. Soit __855cm²__.
La surface occupé par un module 18650 est approximé à 18,3x18,3, soit __334,9mm²__.
Il est donc approximativement possible de disposer __255 éléments__ dans le cadre.

Pour atteindre une autonomie théorique de 70km à 70km/h il faudrait __390 éléments__.
Avec __255 éléments__ nous sommes donc à __65%__ de l'autonomie.

En empilant 2 couches d'éléments 18650 il devient donc possible d'atteindre __510 éléments__, soit __130%__ de l'autonomie cible.

## Caractéristiques du moteur

Le diamètre d'une roue est de __760mm__. Compte tenu de la vitesse que nous souhaitons atteindre, la vitesse de rotation en sortie de transmission sera de __488 tours/minutes__.
En conséquence, le couple nécessaire sera de __57Nm__ en sortie de la transmission.
En combinant ces deux éléments nous retrouvons par ailleurs la puissance calculé précédemment.


