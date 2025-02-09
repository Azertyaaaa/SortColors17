# SortColors17
 # Projet : Trieuse de Pièces par Couleur avec TIA Portal V17

## Description
Ce projet consiste en un programme d'automatisation conçu sous **TIA Portal V17**, permettant de trier automatiquement des pièces en fonction de leur couleur. Le tri est réalisé à l'aide d'un **capteur chromatique** et de **vérins pneumatiques**, qui assurent l'éjection des pièces vers les emplacements correspondants.

## Fonctionnalités
- **Détection de couleur** : Un capteur chromatique analyse la réflexion de la lumière sur les pièces.
- **Transport des pièces** : Une bande transporteuse alimente le système en pièces à trier.
- **Séparation automatique** : Des **vérins pneumatiques** éjectent les pièces vers leurs emplacements respectifs.
- **Surveillance du flux** : Des barrières lumineuses assurent un suivi précis du parcours des pièces.
- **Calibration adaptable** : Possibilité de modifier les valeurs limites pour une meilleure précision du tri.

## Matériel Utilisé
- **Automate Siemens** compatible avec TIA Portal V17
- **Capteur chromatique** pour l'analyse des couleurs
- **Barrières lumineuses** pour détecter le passage des pièces
- **Bande transporteuse** pilotée par un moteur en 24V CC
- **Vérins pneumatiques** commandés par des solénoïdes 3/2 voies
- **Compresseur** pour alimenter le système pneumatique

## Fonctionnement
1. Une pièce est placée sur la bande transporteuse.
2. Elle passe sous un **capteur chromatique**, qui mesure sa réflexion lumineuse et détermine sa couleur.
3. Une **barrière lumineuse** valide la présence de la pièce et active le système d'éjection.
4. Selon la couleur mesurée :
   - Pièce blanche ➔ éjection via **Q3**
   - Pièce rouge ➔ éjection via **Q4**
   - Pièce bleue ➔ éjection via **Q5**
5. La pièce est dirigée vers l'emplacement correspondant.

## Installation
1. Ouvrir **TIA Portal V17**.
2. Importer le projet en chargeant les fichiers fournis.
3. Configurer les entrées/sorties selon le matériel utilisé.
4. Lancer la simulation ou téléverser le programme sur l'API Siemens.

## Fichiers Inclus
- **GrafcetSortColors.dia** : Diagramme GRAFCET du système
- **Programme TIA Portal V17** : Code source du projet
- **Documentation** : Explication du fonctionnement et des valeurs seuils utilisées

## Améliorations Possibles
- Ajout d’un système de **suivi des erreurs** pour détecter les anomalies.
- Intégration d’une **interface HMI** pour ajuster les paramètres de tri.
- Calibration automatique des seuils pour une meilleure précision.

## Auteur
Guillaume

**Licence :** Ce projet est en open source sous licence MIT. Vous êtes libre de le modifier et de le redistribuer.

