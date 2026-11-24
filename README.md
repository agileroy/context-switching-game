# Une chose à la fois · le jeu du context switching

Un jeu en ligne de 15 minutes pour faire ressentir aux équipes le coût du changement de contexte et l'intérêt de se concentrer sur une seule tâche à la fois.

Chaque participant livre trois petits projets à trois clients, trois fois de suite, en changeant seulement sa façon de travailler :

| Manche | Règle | Ce qu'on observe |
| --- | --- | --- |
| 1 · Multitâche | une case de chaque projet à tour de rôle (A, 1, I, B, 2, II…) | les trois clients sont livrés tout à la fin, plus d'erreurs |
| 2 · Focus | un projet entier, puis le suivant | le premier client est livré beaucoup plus tôt, délai moyen en baisse |
| 3 · Focus interrompu | comme la manche 2, avec des messages de collègues auxquels il faut répondre | le coût des interruptions qu'on subit |

Projets : **A** les lettres de A à J, **B** les nombres de 1 à 10, **C** les chiffres romains de I à X.

Jouer : **https://agileroy.github.io/context-switching-game/**

## Animer une session (15 min)

1. **2 min** : chacun ouvre le lien sur son ordinateur ou son téléphone. Ne pas annoncer l'objectif.
2. **6 min** : les trois manches, lancées en même temps par tout le monde.
3. **1 min** : chacun lit ses résultats. Faire remonter quelques chiffres : délai du projet A en manche 1 et 2, délai moyen, erreurs.
4. **6 min** : débrief avec les questions affichées à la fin, conclure sur une action concrète.

Les résultats restent sur l'appareil de chaque joueur (rien n'est envoyé nulle part). Le bouton « Copier mes résultats » permet de les coller dans le chat de la réunion.

## Technique

Un seul fichier `index.html`, sans dépendance ni build. Chaque push sur `main` publie le site sur GitHub Pages via `.github/workflows/deploy.yml`.
