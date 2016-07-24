# dimensionnement

Conditions considérés :
- sol plat
- vent nul
- résistance au roulement négligeable
- condition normal de température et de pression
- densité de l'air = 1.184 (sans unité)
- Cx = 1,2 (celui d'Usain Bolt)
- maitre couple = 0,56m² (source http://cyclurba.fr/velo/666/Cx-SCx-Watts-puissance-vitesse-rendement-aerodynamique.html)
- rendement global = 78%

## puissance mini

### approche par étude des forces

Le moteur doit produire une force de traction égale à la trainé aérodynamique (calcul dans le fichier ods)

Le calcul donne une puissance mini de 3750W en sortie du moteur. Soit 2925W à la roue.

### approche par l'accélération

A partir de la puissance à la roue, nous en déduisons le temps d'accélération mini : 6,46 secondes

## dimensionnement des batteries

Pour une autonomie de 70km il faut donc en théorie 3750Wh d'énergie. En prenant des batteries de 48V cela donne une capacité totale de 78Ah.
Soit 19kg de batterie LiPo en supposant une densité massique de 200Wh/kg.

Ça va être sympa a caser tout ça.
