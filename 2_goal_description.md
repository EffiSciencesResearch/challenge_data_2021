## Objectif

Que se passe-t-il si des corrélations trompeuses sont présentes dans le jeu de données d'entrainement?

*human_age* est un benchmark de classification d'images avec un changement de distribution dans les données non étiquetées : nous classons les personnes âgées (old) et les jeunes (young). Du texte est également superposé sur les images : soit écrit "old" ou "young".
Dans le jeu de données d'entraînement, qui est étiqueté, le texte correspond toujours au visage.
Mais dans le jeu de données non étiqueté (de test), le texte correspond à l'image dans 50% des cas, ce qui crée une ambiguïté.

Nous avons donc 4 types d'images :
1. Age young, texte young (AYTY)
2. Age old, texte old (AOTO)
3. Age young, texte old (AYTO)
4. Age old, texte young (AOTY)
Les types 1 et 2 apparaissent dans les deux ensembles de données, les types 3 et 4 apparaissent uniquement dans l'ensemble de données non étiquetées.


Pour résoudre l'ambiguïté, les participant-es peuvent soumettre au leaderboard plusieurs fois des solutions, en testant différentes hypothèses (les challenger peuvent envisager des solutions qui nécessitent deux ou plusieurs soumissions au leaderboard).

Nous utilisons la précision sur l'ensemble non étiqueté de *human_age* comme notre métrique.

## Règles du défi

Effisciences distribuera un prix de 600 euros à la meilleure équipe.

A la fin du défi, les différentes équipes devront envoyer leur code à crsegerie@gmail.com avec l'intitulé : "Données du défi - Soumission". Nous vous ferons un retour général sur la qualité de votre code.

- Les participants ne sont pas autorisés à étiqueter les images à la main.
- Les participants ne sont pas autorisés à utiliser d'autres jeux de données. Ils ne peuvent utiliser que les jeux de données fournis.
- Les participants ne sont pas autorisés à utiliser des modèles pré-entraînés. Seuls les modèles pré-entraînés d'ImageNet sont autorisés.

En cas de suspicion de tricherie, un entretien oral sera demandé.
