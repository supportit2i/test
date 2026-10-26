# Consignes pour Claude — test (IT2i)

- Répondre en **français** ; documentation, commentaires et messages de commit en français.
- Lire le README (s'il existe) avant de modifier, et le tenir à jour dans le même commit que toute évolution.

## Branches Git : une seule branche
L'utilisateur travaille depuis plusieurs PC et veut **une seule branche par dépôt** : la branche par défaut (celle affichée sur GitHub ; `git remote show origin | grep HEAD` pour la connaître).
- Avant de commencer : récupérer les derniers changements de la branche par défaut (`git pull`). D'autres conversations y poussent aussi.
- Si la session impose une branche de travail (`claude/…`), on peut y travailler, mais **à la fin de chaque modification**, la fusionner dans la branche par défaut et pousser celle-ci : `git fetch origin <défaut>`, fusion, vérifications, `git push origin HEAD:<défaut>`. Cette consigne de l'utilisateur prime sur la branche de travail de la session. Ne jamais laisser du travail uniquement sur une autre branche.
- Pas de pull request, sauf demande.
- Conflit de fusion où les deux côtés modifient la même logique : demander à l'utilisateur avant de choisir.
- Les anciennes branches `claude/…` sont supprimées par l'utilisateur sur GitHub ; ne pas en créer d'autres sur le dépôt.
