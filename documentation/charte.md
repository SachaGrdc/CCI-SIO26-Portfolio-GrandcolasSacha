---
title: Charte
author: Sacha Grandcolas
creator: Typora inc.
subject: Compte-rendu
header:
footer: ${title} - ${author} - Page ${pageNo} / ${totalPages}
---

# Charte

**Date de création** : 27/10/2026 - S.GRANDCOLAS
**Date de modification** : 27/11/2026 - S.GRANDCOLAS
**Sommaire :**

> [TOC]

<div style="page-break-after:always"></div>

## 1. Contexte du projet

Ce portfolio est réalisé dans le cadre de l'atelier de professionnalisation 1 du BTS SIO au CCI Campus Strasbourg. Il présente mon parcours, mes projets et ma veille technologique, en français et en anglais. Il servira de support pour les épreuves du BTS. Cette charte définit le cadre visuel nécessaire à sa réalisation.



## 2. Identité visuelle

J'ai choisi un design épuré avec des couleurs sobres, notamment le brun, le blanc et le gris clair. Le brun sert de couleur principale, tandis que le blanc et le gris clair permettent d'aérer les pages et de séparer les différents contenus. Les titres sont mis en évidence en gras et en majuscules pour faciliter la lecture. La même présentation est reprise sur toutes les pages afin de garder un site cohérent.



## 3. Éléments graphiques

### 3.1. Couleurs

Comme couleur principale, j'utilise du brun : #573F3F

Les fonds des cartes et certains éléments sont en gris pâle : #F4F0F0. J'utilise également du gris clair #D9D9D9 pour différencier certaines parties des pages.

Le fond principal du site reste blanc #FFFFFF

Les paragraphes et les textes classiques sont affichés en noir : #000000

Les titres, sous-titres ainsi que les textes courts et importants sont affichés en brun : #573F3F

Certains textes, notamment ceux présents sur les fonds bruns, sont affichés en gris clair #D9D9D9 afin de conserver un contraste suffisant et de faciliter la lecture.

Lorsque plusieurs cases sont regroupées dans un même bloc, comme sur la page Projets, j'utilise la couleur #D9D9D9 pour le fond qui englobe l'ensemble. Les cases à l'intérieur utilisent la couleur #F4F0F0 afin de les distinguer du fond principal.

Les images qui conservent un fond sont affichées avec des coins arrondis de 20 px tandis que les autres images sont affichées sans fond.



Les contrastes entre les textes et les fonds respectent le minimum d'accessibilité de 4,5:1.

| Texte / fond            | Contraste |
| ----------------------- | --------- |
| `#000000` sur `#FFFFFF` | 21:1      |
| `#573F3F` sur `#FFFFFF` | 9,6:1     |
| `#573F3F` sur `#F4F0F0` | 8,5:1     |
| `#573F3F` sur `#D9D9D9` | 6,8:1     |
| `#D9D9D9` sur `#573F3F` | 6,8:1     |



### 3.2. Typographie

J'utilise la typographie Inter. J'alterne entre l'épaisseur « Bold » pour les titres et les éléments importants et « Regular » pour les paragraphes et les textes secondaires. Les titres sont affichés en gras et en majuscules afin de les faire ressortir.

| Élément    | Épaisseur | Taille ordinateur | Taille mobile |
| ---------- | --------- | ----------------- | ------------- |
| Titre      | Bold      | 60 px             | 32 px         |
| Sous-titre | Bold      | 40 px             | 24 px         |
| Paragraphe | Regular   | 20 px             | 16 px         |
| Bouton     | Regular   | 16 px             | 16 px         |

L'interligne des paragraphes est de 33 px sur ordinateur et de 26 px sur mobile. La police de secours est sans-serif.

### 3.3. Logo, icônes et boutons

J'utilise principalement des logos pour illustrer certaines informations, notamment les établissements scolaires et les outils informatiques. Le logo du portfolio est affiché dans la barre de navigation.

| Élément                     | Forme                                  | Coins arrondis | Bordure |
| --------------------------- | -------------------------------------- | -------------- | ------- |
| Barre de navigation         | Rectangulaire                          | 20 px          | Aucune  |
| Boutons de navigation       | Rectangulaire (Intégrés dans la barre) | 8 px           | Aucune  |
| Cartes                      | Rectangulaire                          | 20 px          | Aucune  |
| Sélecteur de langue         | Rectangulaire                          | 8 px           | 2 px    |
| Pied de page                | Rectangulaire                          | 20 px          | Aucune  |
| Bouton « Mentions légales » | Rectangulaire                          | 8 px           | 2 px    |
| Bouton « Voir plus »        | Rectangulaire                          | 8 px           | 2 px    |
| Images avec fond            | Rectangulaire                          | 20 px          | Aucune  |

Sur ordinateur, les liens de navigation sont disposés horizontalement. Sur mobile, ils sont regroupés dans un menu déroulant accessible avec le bouton « Menu ».

Chaque image possède un texte alternatif.

## 4. Maquettes responsive

## 5. Navigation du site

Le menu de navigation est présent sur toutes les pages du site. Il permet d'accéder aux pages Accueil, Parcours, Projets et Veille technologique. Un sélecteur permet de choisir entre la version française et la version anglaise du site.

Le pied de page contient mon nom ainsi que des liens vers LinkedIn, GitHub et les mentions légales.

### 5.1. Arborescence du site

```
Accueil
├── Parcours
├── Projets
│   ├── La carte électronique
│   ├── Le portfolio
│   ├── Projet AP3
│   └── Projet AP4
├── Veille technologique
└── Mentions légales
```

### 5.2. Parcours utilisateur

Le visiteur arrive sur la page Accueil, il peut consulter le parcours, puis ouvrir la page Projets pour accéder au détail des projets AP3 et AP4. La page Veille technologique est accessible depuis le menu et les mentions légales depuis le pied de page.