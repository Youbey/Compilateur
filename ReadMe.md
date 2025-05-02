# Mini Langage Algorithmique - Interpréteur

Ce projet consiste en la conception et l'implémentation d'un interpréteur pour un langage algorithmique simplifié, développé avec JavaCC.

## 📝 Description

L'objectif de ce projet était de créer un interpréteur pour un langage algorithmique simplifié comprenant :
- Une grammaire formelle définissant la syntaxe du langage
- Un analyseur syntaxique (parser) généré avec JavaCC
- Un système d'exécution pour les programmes écrits dans ce langage
Ce projet applique des concepts de compilation comme l’analyse lexicale, l’analyse syntaxique, et l’interprétation dynamique du code.

## ✨ Fonctionnalités

Le langage supporte les éléments suivants :
- Déclaration de variables (entiers)
- Structures de contrôle :
  - Conditionnelles (`Si...Alors...Sinon...FinSi`)
  - Boucles (`Tanque...Faire...Fait`)
- Opérations arithmétiques de base
- Fonctions d'entrée/sortie :
  - `saisirEntier()`
  - `afficher()`

## 🏗️ Structure du projet
.
├── src/                     # Code source principal

│   ├── Enigme.jj            # Fichier de grammaire JavaCC

│   ├── Parser.java          # Fichiers générés après compilation JavaCC

│   ├── Interpreter.java     # Module d'exécution du langage

│   ├── basic.enigme         # Exemple de programme écrit en langage

│   └── ...                  # Autres fichiers générer nécessaires au projet

├── docs/                    # Documentation technique

└── README.md                # Fichier de présentation du projet

## ⚙️ Installation et utilisation

### Prérequis
- Java JDK (version 8 ou supérieure)
- JavaCC (pour la compilation de la grammaire)

### Compilation
1. Générer le parser à partir de la grammaire :
```bash
javacc Enigme.jj
```
2. Compiler tous les fichiers Java :
```bash
javac *.java
```
Exécution

Pour exécuter un programme écrit dans le langage :
```bash
java Enigme basic.enigme
```
👥 Contribution

Ce projet a été réalisé par Youbey et Mehdi, qui ont travaillé ensemble sur toutes les étapes :

    - Conception et définition de la grammaire du langage

    - Développement du parser et de l’analyse syntaxique

    - Implémentation de l’interpréteur et de l’exécution des instructions

    - Tests et validation du fonctionnement du langage

Ils ont collaboré étroitement pour structurer le projet et garantir son bon fonctionnement.

🔧 Améliorations possibles

    - Ajout du support des chaînes de caractères (String).

    - Optimisation des boucles et des conditions pour améliorer les performances.

    - Extension du langage avec de nouvelles fonctions et types de données.

    - Développement d’une interface graphique pour tester facilement des scripts.
