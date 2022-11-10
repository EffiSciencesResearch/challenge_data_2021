## Objectif

*human_age* est un benchmark de classification d'images avec un changement de distribution dans les données non étiquetées : nous classons les personnes âgées (old) et les jeunes (young). Du texte est également superposé sur les images : soit écrit "old", soit "young".
Dans le jeu de données d'entraînement, qui est étiqueté, le texte correspond toujours au visage.
Mais dans le jeu de données non étiqueté, le texte correspond à l'image dans 50% des cas, ce qui crée une ambiguïté.

Nous avons donc 4 types d'images :
1. Âge jeune, texte jeune (AYTY)
2. Âge avancé, texte avancé (AOTO)
3. Âge jeune, texte vieux (AYTO)
4. Âge avancé, texte jeune (AOTY)
Les types 1 et 2 apparaissent dans les deux ensembles de données, les types 3 et 4 apparaissent uniquement dans l'ensemble de données non étiquetées.


Pour résoudre l'ambiguïté, les participant-es peuvent soumettre au leaderboard plusieurs fois des solutions, en testant différentes hypothèses (une petite poignée de soumission devrait suffire).

Nous utilisons la précision sur l'ensemble non étiqueté de *human_age* comme notre métrique.

## Règles du défi

- Les participants ne sont pas autorisés à étiqueter les images à la main.
- Les participants ne sont pas autorisés à utiliser d'autres jeux de données. Ils ne peuvent utiliser que les jeux de données fournis.
- Les participants ne sont pas autorisés à utiliser des modèles pré-entraînés. Seuls les modèles pré-entraînés d'ImageNet sont autorisés.
