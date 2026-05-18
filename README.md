# 1-Mise-en-place-d-un-r-seau-Active-Directory-sous-VirtualBox

Présentation du projet

Projet réalisé dans le cadre de mon examen réseau de fin de première année en bachelier Informatique de Gestion.

Ce travail consiste à mettre en place une infrastructure réseau Windows complète sous VirtualBox, basée sur Active Directory et Windows Server 2022, dans un environnement proche d’une petite infrastructure d’entreprise réelle.

L’objectif de ce projet n’était pas uniquement de faire fonctionner les différents services, mais surtout de comprendre leur rôle, leur interaction et la logique globale d’une architecture client/serveur professionnelle.

Objectifs du projet

Le projet avait pour objectif de mettre en place :

un serveur Windows Server 2022 ;
un domaine Active Directory ;
un serveur DNS ;
plusieurs postes clients Windows 10 intégrés au domaine ;
une gestion centralisée des utilisateurs et groupes ;
des partages réseau sécurisés ;
des permissions NTFS et permissions de partage ;
des profils itinérants ;
un accès Internet des clients via le serveur grâce au routage NAT ;
un déploiement automatisé de logiciels via les stratégies de groupe (GPO).
Technologies et services utilisés
Virtualisation
Oracle VirtualBox
Systèmes d’exploitation
Windows Server 2022
Windows 10
Services Windows
Active Directory Domain Services (AD DS)
DNS
Routage et accès distant (NAT)
Stratégies de groupe (GPO)
Administration
Gestion des utilisateurs et groupes
Permissions NTFS
Partages réseau
Profils itinérants
Fonctionnalités mises en place
Active Directory

Création d’un domaine :

entreprise.local

avec :

authentification centralisée ;
gestion des utilisateurs ;
gestion des groupes ;
gestion des ordinateurs du domaine.
Intégration des postes clients

Les postes Windows 10 ont été :

configurés en IP statique ;
reliés au DNS du serveur ;
intégrés au domaine Active Directory.
Profils itinérants

Les utilisateurs retrouvent automatiquement :

leur bureau ;
leurs fichiers ;
leurs paramètres ;

sur n’importe quel poste du domaine.

Les profils sont centralisés sur le serveur.

Partages réseau sécurisés

Mise en place :

d’un dossier partagé réseau ;
des permissions de partage ;
des permissions NTFS.

Le projet met en évidence la différence importante entre :

permissions réseau ;
permissions NTFS.
Accès Internet via le serveur (NAT)

Les postes clients accèdent à Internet :

au travers du serveur

grâce au service :

Routage et accès distant (NAT)

Cette architecture permet :

une meilleure centralisation ;
un meilleur contrôle réseau ;
une approche plus professionnelle de l’infrastructure.
Déploiement logiciel par GPO

Déploiement automatique de :

VLC Media Player

sur les postes clients grâce aux :

Stratégies de groupe (GPO)

sans installation manuelle sur chaque machine.

Documentation du projet

La documentation contient :

toutes les étapes détaillées ;
les explications techniques ;
les choix de configuration ;
les captures d’écran ;
les tests de validation ;
les problèmes rencontrés et leur résolution.

L’objectif était de produire :

un support de compréhension personnel ;
un guide réutilisable ;
un tutoriel pédagogique pour d’autres étudiants ;
une démonstration de mes compétences techniques.
Ce que ce projet m’a apporté

Ce projet m’a permis de développer une compréhension concrète :

des infrastructures Windows ;
du fonctionnement d’Active Directory ;
de l’administration réseau ;
des permissions Windows ;
des GPO ;
du routage NAT ;
et de la logique client/serveur en environnement professionnel.

Il m’a également appris à :

analyser des problèmes techniques ;
comprendre les interactions entre les services ;
documenter proprement une infrastructure ;
travailler avec rigueur et méthode.
Auteur
Younes Andaloussi

Étudiant en Bachelier Informatique de Gestion
Projet réseau — Examen de fin de première année
