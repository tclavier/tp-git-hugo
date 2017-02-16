+++
date = "2017-02-14T12:00:00+02:00"
title = "Sujet de TP"

+++

# Mémo

## Hugo

Création d'un article

    ./bin/hugo new nom-de-l-article.md

Lancer Hugo sur son poste de dev

    ./bin/hugo server --buildDrafts -w

Puis visitez http://localhost:1313/

## Markdown

    # Titre 1
    ## Sous Titre 1

    * Liste à puce, item1
    * Liste à puce, item2

    *Italique*
    **Gras**
    ***Gras et italique***

# Exercices

Dans les exercices suivants, je vous invites à systématiquement observer l'état de votre espace de travail à l'aide de la commande `git status`. et à surveiller l'historique avec la commande `git log --oneline --decorate --graph --all`

## Configuration

* Configurer son nom, prénom et email à l'aide de la commande `config`
* Configurer le serveur mandataire de l'université (`http://cache.univ-lille1.fr:3128`)
* Vérifiez à l'aide de la commande `git config --list`

## Les débuts (add, commit, pull, push, status)

* Créer puis indexer chacun un article. Faire un premier commit. En utilisant du Markdown vous pouvez affiner la mise en page.
* Partager l’article.
* Récupérer les articles depuis son poste.
* Jouer avec les commandes `add`, `commit`, `pull`, `push`, `status`

## Gestion des conflits (add, commit, pull, push)

Par équipe de 2 à 4, définir un sujet d’article et un nom de fichier associé. Pour cet éxercice, vous ne modifierez que ce fichier.

* Modifier en même temps l’article de son groupe de travail.
* Partager ses modifications à plusieurs reprises.
* Expérimenter différents conflits (en haut du fichier, en bas du fichier, une ligne, de nombreuses lignes, etc.)

## Ignorer des fichiers (.gitignore, clean)

* Relancez Hugo avec les options : `server --buildDrafts -w -d public`
* Modifier .gitignore pour que les fichiers générer par Hugo soient ignoré par Git
* Nettoyer son répertoire de travail avec la commande `clean`.

## Visualiser l’historique (blame, diff, log, show)

* Afficher l’historique des commits.
* Afficher la différence entre deux commits.
* Afficher le détail d'un commit.
* Identifier l’auteur des différentes parties de son article.
* Expérimenter l’affichage de l’historique avec différentes options de formatage.
* Rajouter l'alias `h` pour les options `log --oneline --decorate --graph --all`

## Des changements plus évolués (mv, reset, rm)

* Renomer un article personnel et enregistrer ce changement de 2 façon différentes.
* Faire un changement et le valider avant de l'annuler définitivement.
* Ajouter un fichier, le valider puis le supprimer.

## Manipulation des branches

* Créer une branche `feature_123`
* Vérifier l’existence de cette branche
* Changer de branche
* Créer une autre branche à votre nom et se placer directement dessus.
* Supprimer la branche `feature_123`
* Comprendre et tester les commandes `checkout` et `branch`

## Fusion de branches locales et distantes

* Effectuer plusieurs commits sur la branche créée précédemment.
* Pousser cette branche sur le serveur GitLab
* Fusionner cette branche avec la branche master
* Récupérer les branches des autres participants
* Fusionner la nouvelle branche avec la branche origin (serveur)

## Tags : Manipulation et partage

* Placer un tag sur un commit
* Pousser ce tag sur le serveur
* Récupérer et lister les tags des participants

## Remonter le temps (checkout, revert)

* Se positionner dans sa branche
* Repositionner HEAD dans un état antérieur
* Choisir un commit, puis supprimer tous les commits postérieurs à celui-ci.
* Annuler, sans les perdre, un ou plusieurs commits.

## Rebase de branche

* Créer une branche locale de type feature à votre nom
* Effectuer plusieurs commits
* Réappliquer les commits dans master via un `rebase`
* Expliquez ce que fait un `pull -r` et dans quel contexte l'utiliser.

## Mettre de côté ses développements

* Effectuer de nouvelles modifications (sans commit) sur sa branche.
* Mettre de côté son travail à l'aide de la commande `stash` et effectuer une modification (sur le même fichier).
* Une fois la modification partagé, reprendre son travail mis de côté.

## Réécrire l'histoire !

 * Prendre un commit quelconque et l’appliquer localement
 * Fusionner deux commits en un seul.
 * Changer le commentaire d’un commit
