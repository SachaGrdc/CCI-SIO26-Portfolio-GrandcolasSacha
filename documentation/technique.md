---
title: Technique
author: Sacha Grandcolas
creator: Typora inc.
subject: Compte-rendu
header:
footer: ${title} - ${author} - Page ${pageNo} / ${totalPages}

---

# Technique

**Date de création** : 16/10/2026 - S.GRANDCOLAS
**Date de modification** : 27/11/2026 - S.GRANDCOLAS
**Version** : 1.0

**Sommaire :**

> [TOC]

<div style="page-break-after:always"></div>

## 1. Les outils

Afin de pouvoir travailler sur ce projet, j'ai utilisé plusieurs outils : 

**WSL** : C'est une sorte de "machine virtuelle" Linux connectée à Windows et qui a pour but de pouvoir utiliser l'environnement Linux directement via Windows, j'utilise Ubuntu 26.04 LTS comme OS, WSL est en version 3.0.3

**Windows** : C'est le système d'exploitation principal que j'utilise, plus exactement j'utilise la version 26H2

**Visual Studio Code** : C'est l'éditeur de code que j'utilise afin de pouvoir coder, la version est en 1.146.0

**Typora** : C'est l'éditeur Markdown qui me permet de rédiger toute la documentation, celui-ci est en version 1.14.15

**Apache** : C'est un logiciel qui sert à héberger et diffuser des sites web, j'utilise la version 2.4.66 de Apache2, je l'ai installé dans WSL.

**Brave** : Le navigateur qui me permet de tester l'affichage du site web, celui-ci est en version 1.100.58

**Git** : C'est un logiciel de gestion de versions qui permet de suivre l'ensemble des modifications d'un projet, j'utilise la version 2.53.0 dans WSL et la version 2.56.0 dans Windows.

**GitHub** : C'est une plateforme qui permet d'héberger des projets informatiques et de partager leur code source. Je l'utilise pour stocker mon portfolio et conserver son historique de modifications.

**Figma** : C'est un outil qui permet de structurer des pages web en faisant des maquettes, je l'utilise pour créer les différentes pages de mon portfolio, j'utilise la version web.

**SSH** : C'est un protocole réseau sécurisé qui permet de se connecter à distance à un appareil (ordinateur ou serveur) et d'y exécuter des commandes via une connexion chiffrée, j'utilise ce protocole pour envoyer les commits sur GitHub.



**Justification des choix** : WSL est plus léger qu'une machine virtuelle et intégré à Windows. Visual Studio Code est gratuit et compatible avec WSL. Typora permet de voir directement le rendu Markdown et de l'exporter en PDF. Apache est gratuit et connu. Brave est un navigateur basé sur Chromium, il est donc compatible avec la majorité des sites web. Git et GitHub conservent l'historique et une copie en ligne du projet. Figma permet de créer les maquettes dans le navigateur. SSH assure une connexion chiffrée à GitHub.

<div style="page-break-after:always"></div>

## 2. Les langages et technologies

Afin de développer les différentes pages du portfolio je vais devoir utiliser plusieurs langages, tout d'abord le HTML, c'est ce qui permet de structurer le contenu des pages web, j'utilise HTML5. Une fois la structure des pages faite, il faut mettre en forme celles-ci, c'est pourquoi j'utilise CSS, plus exactement CSS3, je l'utilise pour gérer les couleurs, les polices, la taille des images ainsi que la disposition des différents éléments. Enfin, pour ajouter des animations et rajouter de l'interactivité le JavaScript est très utile.

<div style="page-break-after:always"></div>

## 3. Architecture de l'environnement

### 3.1. Présentation de l'environnement

Pour réaliser ce portfolio, j'utilise Windows 11 comme système d'exploitation mais pour pouvoir utiliser l'environnement Linux j'utilise également WSL avec Ubuntu 26.04 LTS.

Apache est installé dans Ubuntu et permet de diffuser les pages web en local. Les fichiers du portfolio sont accessibles depuis cet environnement et peuvent être modifiés avec Visual Studio Code.

Une fois Apache lancé je peux accéder au site depuis mon navigateur Brave afin de vérifier son affichage et de tester les différentes pages.

### 3.2. Organisation du projet

Le projet est organisé dans plusieurs dossiers afin de séparer les différents éléments.

Le dossier documentation contient les fichiers Markdown utilisés pour préparer le portfolio notamment le contenu, la charte graphique et la documentation technique. Il contient aussi un dossier medias pour rassembler les illustrations utilisées dans les documents.

Les fichiers du site web seront regroupés dans un dossier dédié avec les pages HTML, les fichiers CSS, le JavaScript et les images utilisées sur le site.

Voici l'ensemble de l'arborescence du projet : 

```
portfolio/
├── .git/
├── README.md
├── documentation/
│   ├── charte.md
│   ├── contenu.md
│   ├── technique.md
│   └── medias/
└── html/
    ├── index.html
    └── assets/
        ├── fonts/
        ├── css/
        │   └── style.css
        ├── js/
        │   └── main.js
        └── img/
```

Cette arborescence se trouve dans WSL à l'emplacement suivant : /var/www/html/portfolio 



### 3.3. Gestion et suivi du projet

Pour suivre l'évolution du portfolio j'utilise Git et GitHub.

Git me permet d'enregistrer les différentes modifications apportées au projet grâce aux commits. GitHub me permet de conserver une copie du projet en ligne et de retrouver mes modifications.

Voici les commandes utilisées pour le suivi de version :

```bash
git add .                           # sélectionne les fichiers modifiés
git commit -m "Message"				# enregistre les modifications avec un message
git push                            # envoie les commits sur GitHub
```

```bash
git clone git@github.com:SachaGrdc/CCI-SIO26-Portfolio-GRANDCOLASSacha.git   # récupère le projet depuis GitHub
```



### 3.4. Installation de l'environnement

```bash
wsl --install -d Ubuntu-26.04        # dans PowerShell
sudo apt update                      # puis dans Ubuntu
sudo apt install apache2 openssh-client
sudo systemctl start apache2
ssh-keygen -t ed25519                # ajouter ensuite la clé publique sur GitHub
ssh -T git@github.com                # test de la connexion
```

Il n'est pas nécessaire d'installer Git car il est installé par défaut sur Ubuntu 26.04.



### 3.5. Droits d'accès

```bash
sudo chown -R root:adm /var/www       # propriétaire root, groupe adm
sudo chmod 2775 /var/www              # écriture pour root et adm, groupe hérité
sudo chmod 2775 /var/www/html         # mêmes droits pour le dossier web
sudo chmod 664 /var/www/html/*        # écriture pour root et adm, lecture pour les autres
```



### 3.6. Sécurité

- La clé SSH privée reste sur mon poste et n'est jamais ajoutée au dépôt.
- Apache n'a aucun droit d'écriture sur le projet.
- Les logiciels sont mis à jour régulièrement.



