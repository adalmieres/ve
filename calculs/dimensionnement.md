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

Le calcul donne une puissance mini de 3750W en sortie du moteur. Soit 2925W à la roue.

### Approche par l'accélération

A partir de la puissance à la roue, nous en déduisons le temps d'accélération mini : 6,46 secondes

## Dimensionnement des batteries

Pour une autonomie de 70km il faut donc en théorie 3750Wh d'énergie. En prenant des batteries de 48V cela donne une capacité totale de 78Ah.
Soit 19kg de batterie LiPo en supposant une densité massique de 200Wh/kg.

Autre approche possible : partir de l'espace disponible et en déduire la quantité embarquable.

### Capacité embarquable

Supposons l'emplois de module lithium 18650 (cylindre d'un diamètre de 18,3mm) disposé en pavage carré sur la surface de l'intérieur du cadre.
Le cadre est approximé à un triangle de base 450mm et de hauteur 380mm.
La surface est donc de 85500mm². Soit 855cm².
La surface occupé par un module 18650 est approximé à 18,3x18,3, soit 334,9mm².
Il est donc approximativement possible de disposer 255 éléments dans le cadre.

Pour atteindre une autonomie théorique de 70km à 70km/h il faudrait 390 éléments.
Avec 255 élément nous sommes donc à 65% de l'autonomie.

En empilant 2 couches d'éléments 18650 il devient donc possible d'atteindre 510 éléments, soit 130% de l'autonomie cible.

## Caractéristiques du moteur

Le diamètre d'une roue est de 760mm. Compte tenu de la vitesse que nous souhaitons atteindre, la vitesse de rotation en sortie de transmission sera de 488 tours/minutes.
En conséquence, le couple nécessaire sera de 57Nm en sortie de la transmission.
En combinant ces deux éléments nous retrouvons par ailleurs la puissance calculé précédemment.


