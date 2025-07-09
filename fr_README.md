# Commande Articulaire d'un Manipulateur Robotique de Type RP
Ce projet se concentre sur la simulation de diverses stratégies de contrôle pour un manipulateur robotique simple de type RP en utilisant MATLAB-SIMULINK. L'objectif est de développer et tester des schémas de contrôle pour les variables articulaires du robot afin de suivre des trajectoires prédéfinies.
## Aperçu
Le manipulateur se compose de :
- **Articulation Rotative (R) :** Permet au premier lien de tourner autour de l'axe vertical.
- **Articulation Prismatique (P) :** Permet le mouvement linéaire du deuxième lien.
L'objectif est de contrôler les variables q1(t) et q2(t) pour suivre des profils prédéfinis combinant accélération uniforme, vitesse constante et décélération uniforme. Les configurations désirées pour le manipulateur commencent à (q1(t0) = 0, q2(t0) = 0.5) et se terminent à (q1(t1) = π/2, q2(t1) = 1).
## Composants Principaux
1. **Modèle Dynamique :** Inclut les effets d'inertie, de Coriolis, centrifuges et gravitationnels.
2. **Actionneurs :** Représentés avec des paramètres comme le couple moteur, les rapports de réduction et l'inertie effective.
3. **Stratégies de Contrôle :** 
   - **Contrôle PD :** Évalué pour divers rapports de réduction afin d'optimiser la stabilité et les performances du système.
   - **Contrôle PID :** Précision améliorée grâce à l'action intégrale.
   - **Contrôle Centralisé Non-linéaire :** Incorpore des stratégies de feedforward pour un meilleur suivi de trajectoire.
   - **Contrôle Linéarisant Découplé :** Implémente des boucles imbriquées pour une meilleure linéarité et découplage.
## Tâches Réalisées
- Implémentation de différentes lois de contrôle sous modèles linéaires et non-linéaires.
- Simulation des réponses du système dans MATLAB-SIMULINK sous conditions variables (par ex. effets gravitationnels, perturbations).
- Analyse des effets de différents rapports de réduction et paramètres de contrôleur sur les performances du système.
## Outils Utilisés
- **MATLAB-SIMULINK :** Pour la modélisation et simulation du manipulateur robotique.
- **S-Functions Personnalisées :** Développées pour implémenter des lois de contrôle avancées, incluant anticipation centralisée et découplage.
## Résultats
Ce projet fournit une compréhension approfondie des stratégies de contrôle articulaire pour les manipulateurs RP, mettant en évidence les compromis entre approches de contrôle linéaires et non-linéaires et leur impact sur la précision, stabilité et robustesse.
---
N'hésitez pas à explorer les fichiers de simulation et modifier les paramètres de contrôle pour observer leurs effets sur le comportement du manipulateur.
