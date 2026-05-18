<h1 align="center">Mise en place d'un réseau Active Directory sous VirtualBox</h1>

<p align="center">
  <strong>Projet réseau — Examen de fin de première année</strong><br>
  Bachelier Informatique de Gestion
</p>

<p align="center">
  <img alt="Windows Server 2022" src="https://img.shields.io/badge/Windows%20Server-2022-0078D4?style=for-the-badge&logo=windows&logoColor=white">
  <img alt="Active Directory" src="https://img.shields.io/badge/Active%20Directory-AD%20DS-2F6DB3?style=for-the-badge">
  <img alt="VirtualBox" src="https://img.shields.io/badge/VirtualBox-Lab-183A61?style=for-the-badge&logo=virtualbox&logoColor=white">
</p>

---

## Présentation du projet

Ce projet a été réalisé dans le cadre de mon examen réseau de fin de première année en bachelier Informatique de Gestion.

Il consiste à mettre en place une infrastructure réseau Windows complète sous VirtualBox, basée sur Active Directory et Windows Server 2022, dans un environnement proche d'une petite infrastructure d'entreprise réelle.

L'objectif n'était pas uniquement de faire fonctionner les différents services, mais surtout de comprendre leur rôle, leur interaction et la logique globale d'une architecture client/serveur professionnelle.

## Objectifs du projet

Le projet avait pour objectif de mettre en place :

- un serveur Windows Server 2022 ;
- un domaine Active Directory ;
- un serveur DNS ;
- plusieurs postes clients Windows 10 intégrés au domaine ;
- une gestion centralisée des utilisateurs et des groupes ;
- des partages réseau sécurisés ;
- des autorisations NTFS et des autorisations de partage ;
- des profils itinérants ;
- un accès Internet des clients via le serveur grâce au routage NAT ;
- un déploiement automatisé de logiciels via les stratégies de groupe (GPO).

## Technologies et services utilisés

| Catégorie | Éléments utilisés |
|---|---|
| Virtualisation | Oracle VirtualBox |
| Systèmes d'exploitation | Windows Server 2022, Windows 10 |
| Services Windows | AD DS, DNS, RRAS/NAT, GPO |
| Administration | Utilisateurs, groupes, permissions NTFS, partages réseau, profils itinérants |

## Fonctionnalités mises en place

### Active Directory

Création d'un domaine :

```text
entreprise.local
```

avec :

- authentification centralisée ;
- gestion des utilisateurs ;
- gestion des groupes ;
- gestion des ordinateurs du domaine.

### Intégration des postes clients

Les postes Windows 10 ont été :

- configurés en IP statique ;
- connectés au DNS du serveur ;
- intégrés au domaine Active Directory.

### Profils itinérants

Les utilisateurs récupèrent automatiquement :

- leur bureau ;
- leurs fichiers ;
- leurs paramètres ;

sur n'importe quel poste du domaine.

Les profils sont centralisés sur le serveur.

### Partages réseau sécurisés

Mise en place :

- d'un dossier réseau partagé ;
- des autorisations de partage ;
- des autorisations NTFS.

Le projet met en évidence la différence importante entre :

- autorisations réseau ;
- autorisations NTFS.

### Accès Internet via le serveur

Les postes clients accèdent à Internet :

```text
PC client -> Serveur Windows -> NAT -> Internet
```

grâce au service :

```text
Routage et accès distant (NAT)
```

Cette architecture permet :

- une meilleure centralisation ;
- un meilleur contrôle réseau ;
- une approche plus professionnelle de l'infrastructure.

### Déploiement logiciel par GPO

Déploiement automatique de :

```text
VLC Media Player
```

sur les postes clients grâce aux :

```text
Stratégies de groupe (GPO)
```

sans installation manuelle sur chaque machine.

## Documentation du projet

La documentation complète contient :

- toutes les étapes détaillées ;
- les explications techniques ;
- les choix de configuration ;
- les captures d'écran ;
- les tests de validation ;
- les problèmes rencontrés et leur résolution.

Consulter la documentation complète :

[documentation.md](documentation.md)

## Ce que ce projet m'a apporté

Ce projet m'a permis de développer une compréhension concrète :

- des infrastructures Windows ;
- du fonctionnement d'Active Directory ;
- de l'administration réseau ;
- des autorisations Windows ;
- des GPO ;
- du routage NAT ;
- de la logique client/serveur en environnement professionnel.

Il m'a également appris à :

- analyser des problèmes techniques ;
- comprendre les interactions entre les services ;
- documenter proprement une infrastructure ;
- travailler avec rigueur et méthode.

## Auteur

<p align="center">
  <strong>Younes Andaloussi</strong><br>
  Étudiant en Bachelier Informatique de Gestion<br>
  Projet réseau — Examen de fin de première année
</p>
