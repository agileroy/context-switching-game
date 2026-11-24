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

## Deux modes

- **Jouer seul** : pour découvrir le jeu ou le tester avant un atelier.
- **En équipe** : l'animateur crée une salle et partage le lien ou le QR code. Chacun joue de son côté, à son rythme ; les plus rapides patientent sur un écran d'attente. Quand tout le monde a terminé, l'animateur révèle les résultats de l'équipe, affichés en même temps chez tous : médianes par manche, part des participants ralentis par les interruptions, et un nuage de points où chacun retrouve son parcours (les autres restent anonymes).

## Animer une session en équipe (15 min)

1. **2 min** : créer une salle et projeter son écran. Chacun ouvre le lien ou scanne le QR code et entre son prénom. Ne pas annoncer l'objectif.
2. **6 min** : chacun joue les trois manches. L'écran animateur montre l'avancement de chacun.
3. **1 min** : quand tout le monde a terminé, cliquer sur « Révéler les résultats de l'équipe ».
4. **6 min** : débrief avec le nuage de points et les questions proposées, conclure sur une action concrète.

## Technique

Un seul fichier `index.html`, sans build. Le mode équipe utilise Firebase Realtime Database (connexion anonyme), chargé depuis le CDN de Firebase uniquement quand on crée ou rejoint une salle.

Le projet Firebase `limit-wip-vleroy` est partagé avec [Rush en cuisine](https://github.com/agileroy/wip-limit-game) : les règles de sécurité de ce jeu sont dans la section `csRooms` de son fichier `database.rules.json`, publié par son workflow. Chaque joueur n'écrit que ses propres résultats ; seul l'animateur peut révéler les résultats ou retirer un participant. Chaque push sur `main` publie le site sur GitHub Pages via `.github/workflows/deploy.yml`.
