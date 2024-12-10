
README - Simulateur de Board de Jeu 🛡️🎮

Ce projet implémente une classe Board, conçue pour gérer et simuler un plateau de jeu basé sur un thème historique ou mythologique. Il inclut des mécaniques de tour par tour, des unités, des terrains variés et des interactions entre ces éléments. Ce document fournit une vue d'ensemble des fonctionnalités et de l'utilisation de cette classe.

⚙️ Fonctionnalités Principales
1. Plateau de Jeu
Dimensions : Le plateau mesure 9 lignes par 20 colonnes.
Terrain : Chaque case est initialisée aléatoirement comme une forêt (🌳) ou un champ (🌾), et peut contenir une unité ou rester vide.
2. Gestion des Tours
Chaque joueur joue à tour de rôle :
Gaulois : Jouent aux tours pairs.
Romains : Jouent aux tours impairs.
Le numéro du tour (lv) suit le déroulement de la partie.
3. Types de Terrains et Unités
Terrains :

Champ (Field) : Représenté par des cases vertes.
Forêt (Forest) : Représenté par des cases vert foncé.
Rivière (River) : Représenté par des cases bleues.
Unités : Chaque unité a un rôle spécifique et des actions distinctes :

Gaulois : Asterix, Obelix, Idefix.
Romains : Caesar, Roman, RomanCamp.
4. Interactions et Mécaniques
Les unités peuvent se déplacer, interagir avec d'autres unités ou le terrain selon leurs rôles spécifiques.
Les tours sont gérés automatiquement et des piles de mouvements permettent de suivre l’historique des actions.
🛠️ Description des Méthodes
Constructeur Board
Initialise un plateau avec un générateur aléatoire (grâce à une graine seed).
Place aléatoirement les types de terrains sur le plateau.
Méthodes Clés
raman()

Affiche l’état actuel du plateau, le tour en cours et les unités positionnées.
amzing()

Met à jour les unités sur le plateau en fonction des règles du jeu.
Passe au tour suivant.
mov(Difficulty d)

Configure le plateau pour différents niveaux de difficulté :
Tinydefix : Scénario de petite difficulté avec peu d'unités.
Grobelix : Scénario avancé avec davantage d'unités et d'obstacles.
oups()

Annule les derniers mouvements effectués.
Permet de revenir en arrière dans la partie.
terminal()

Affiche l'historique des mouvements effectués pendant la partie.
