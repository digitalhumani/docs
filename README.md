# Raas API

La documentation de l'API RaaS est générée à l'aide de l'outil [Jekyll](https://jekyllrb.com/). Celui-ci permet de générer des fichiers html à l'aide de fichiers de format markdown.

Ce modèle a été construit par [CloudCannon](http://cloudcannon.com/).

## Étapes pour commencer à travailler sur la documentation

  1. Installer [Ruby](https://www.ruby-lang.org/en/)
  2. Installer [Jekyll](https://jekyllrb.com/)
  3. Clôner le projet

## Modifications de la documentation actuelle

Afin d'ajouter une nouvelle section à la documentation ou de modifier une section actuelle, il ne suffit que d'ajouter ou de modifier un fichier markdown dans l'un des dossiers représentant une collection.

La documentation actuelle contient les trois collections suivantes 
* Documentation
* API
* Appendix

Afin que le fichier soit traité par Jekyll, celui-ci doit débuter par un bloc front matter. Voir les fichiers actuellement en place comme exemple ou la documentation suivante

[Jekyll Front Matter](https://jekyllrb.com/docs/front-matter/)

**Note**: Ne pas travailler ou effectuer de changements sur les fichiers situés dans le dossier *_site*. Il s'agit des fichiers générés par Jekyll, alors toutes les modifications effectuées sur les fichiers situés de ce dossier seront perdues lorsque le serveur sera démarré. 

### Information sur la structure des collections de la documentation

* Chaque section de la documentation est une collection différente. Cela aide à organiser le contenu.
* L'ordre des collections est déterminé par les champs position_number dans la configuration des collections dans le fichier `_config.yml`.
* L'ordre des éléments d'une collection est déterminé par le champ position_number dans un bloc front matter dans un fichier markdown, par exemple `introduction.md`.

## Démarrer le serveur

Installer les dépendances du Gemfile avec [Bundler](http://bundler.io/):

~~~bash
$ bundle install
~~~

Pour rapidement voir les changements effectués sur l'adresse [localhost:4000](http://localhost:4000.com), excécuter  la commande `Jekyll` suivante à l'aide de `Bundle`:

~~~bash
$ bundle exec jekyll serve
~~~

## Déploiement des modifications

Actuellement, les modifications sont manuellement transférées du dossier *_site* au compartiment S3 sur AWS. Les fichiers à transférer sont les suivants
* css/style.css
* favicon.png
* images/logo.svg
* index.html
* js/main.js