---
title: Technique
author: Sacha Grandcolas
creator: Typora inc.
subject: Compte-rendu
header:
footer: ${title} - ${author} - Page ${pageNo} / ${totalPages}

---

# La technique

**Date de création** : 16/10/2026 - S.GRANDCOLAS
**Date de modification** : 11/11/2026 - S.GRANDCOLAS
**Sommaire :**

> [TOC]

<div style="page-break-after:always"></div>
<div style="page-break-after:always"></div>

## 1. Les outils

Afin de pouvoir travailler sur ce projet j'ai utilisé plusieurs outils : 

**WSL** : C'est une sorte de "machine virtuelle" linux connecté à Windows et qui a pour but de pouvoir utiliser l'environnement linux directement via Windows, j'utilise Ubuntu 26.04 LTS comme OS

**Windows** : C'est le système d'exploitation principal que j'utilise, plus exactement j'utilise la version 26h2

**Visual Studio Code** : C'est l'éditeur de code que j'ai utilisé afin de pouvoir coder

**Typora** : C'est l'éditeur Markdown qui m'a permis de rédiger toute la documentation

**Apache** : C'est un logiciel qui sert à héberger et diffuser des sites web, j'utilise la version 2.4.66 de Apache2, je l'ai installé dans WSL

**Brave** : Le navigateur qui me permet de tester l'affichage du site web

**Git** : C'est un logiciel de gestion de versions qui permet de suivre l'ensemble des modifications d'un projet, j'utilise la version 2.53.0 dans WSL et la version 2.56.0 dans Windows

**GitHub** : C'est une plateforme qui permet d'héberger des projets informatiques et de partager leur code source. Je l'utilise pour stocker mon portfolio et conserver son historique de modifications

**Figma** : C'est un outil qui permet de structurer des pages web en faisant des maquettes, je l'utilise pour créer les différentes pages de mon portfolio



## 2. Les langages et technologies

Afin de développer les différentes page du portfolio je vais devoir utiliser plusieurs langages, tout d'abord le HTML, c'est ce qui qui permet de structurer le contenu des pages web, j'utilise HTML5. Une fois la structure des pages fait, il faut mettre en forme celles-ci, c'est pourquoi j'utilise CSS, plus exactement CSS3, je l'utilise pour gérer les couleurs, les polices, la taille des images ainsi que la disposition des différents éléments. Enfin, pour ajouter des animations et rajouter de l'interactivité le JavaScript est très utile 



## 3. Architecture de l'environnement

### 3.1. Présentation de l'environnement

Pour réaliser ce portfolio, j'utilise Windows 11 comme système d'exploitation mais pour pouvoir utiliser l'environnement linux j'utilise également WSL avec Ubuntu 26.04 LTS

Apache est installé dans Ubuntu et permet de diffuser les pages web en local. Les fichiers du portfolio sont accessibles depuis cet environnement et peuvent être modifiés avec Visual Studio Code

Une fois Apache lancé je peux accéder au site depuis mon navigateur Brave afin de vérifier son affichage et de tester les différentes pages.

### 3.2. Organisation du projet

Le projet est organisé dans plusieurs dossiers afin de séparer les différents éléments.

Le dossier documentation contient les fichiers Markdown utilisés pour préparer le portfolio notamment le contenu, la charte graphique et la documentation technique. Il contient aussi un dossier medias pour rassembler les illustrations utilisées dans les documents.

Les fichiers du site web seront regroupés dans un dossier dédié avec les pages HTML, les fichiers CSS, le JavaScript et les images utilisées sur le site.

Voici l'ensemble de l'arborescence du projet : 

portfolio/
├── README.md
├── documentation/
│   ├── charte.md
│   ├── contenu.md
│   ├── technique.md
│   └── medias/
└── html/
    ├── index.html
    └── assets/
        ├── css/
        │   └── style.css
        ├── js/
        │   └── main.js
        └── img/



Cette arborescence se trouve dans l'emplacement suivant : /var/www/html/portfolio 

### 3.3. Gestion et suivi du projet

Pour suivre l'évolution du portfolio j'utilise Git et GitHub

Git me permet d'enregistrer les différentes modifications apportées au projet grâce aux commits. GitHub me permet de conserver une copie du projet en ligne et de retrouver mes modifications.



