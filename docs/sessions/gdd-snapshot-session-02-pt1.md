# GDD Snapshot — Session 02 Partie 1

> Snapshot des décisions de design figées en Session 02 Partie 1 (14 mai 2026).
> Toute la doc vivante est dans Notion. Ceci est juste une trace git.

## Pitch officiel

One Piece RP est un arena fighter PvP nerveux en 1v1 / 2v2, où chaque joueur choisit sa classe de combattant (épéiste, poings, pieds, tireur d'élite) et personnalise son apparence (nom, couleur).

Le cœur du jeu : enchaîner des combos visuellement impressionnants, exploiter les synergies entre classes en duo, et récompenser les joueurs qui theorycraftent leurs builds.

Cible : un groupe d'amis fans de One Piece et de PvP technique, qui veulent un jeu pour soirées entre potes.

Note : le nom "One Piece RP" est conservé car l'inspiration thématique reste One Piece, mais les personnages sont génériques (pas de Luffy, Zoro, etc.).

## Décisions de design fondatrices

- Référence gameplay : Fighting game / Smash Bros
- Cible : fans One Piece + amateurs PvP technique
- Système de classes : 4 classes au MVP (Épéiste, Poings, Pieds, Tireur d'élite)
- Personnalisation MVP : nom + couleur uniquement
- Fruits du Démon : pas au MVP, ajoutés en V2+
- Condition de victoire : First to 5 kills par round
- Format match : Best of 3 rounds (5-7 min total)
- Mode unique au MVP : respawn rapide (3-5 sec)
- Pas de mode élimination au MVP (→ V2)
- Pas de persistance MVP (nom/couleur en mémoire match)
- Diffusion : privé entre potes, pas de Steam

## Les 4 classes du MVP

| Classe | Style | Portée | Mobilité | Vie | Inspiration |
|---|---|---|---|---|---|
| Épéiste | Mêlée précise | Moyenne | Moyenne | Moyenne | Zoro, Mihawk |
| Poings | Mêlée brute | Courte | Faible | Haute | Garp, Akainu |
| Pieds | Mêlée mobile | Courte | Haute | Faible | Sanji, Lucci |
| Tireur d'élite | Distance | Longue | Faible | Faible | Usopp, Yasopp |

Triangle classique : Force / Vitesse / Distance.

## Core loop MACRO

Lancement → menu → invitation pote (2v2) ou solo (1v1) → personnalisation + choix classe → arène → match → écran fin → rejouer.

## Core loop MICRO (par round)

Spawn → countdown → combat libre → kills (respawn 3-5s) → first to 5 kills gagne le round → best of 3 gagne le match.

## À venir (Session 02 Partie 2)

- Capacités détaillées de chaque classe (3 capacités + 1 attaque de base)
- Chiffres du combat (PV, dégâts, cooldowns)
- Map MVP (taille, thème, layout)
- UI MVP
- Système d'invitation entre amis