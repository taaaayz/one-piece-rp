# Session 01 — Setup environnement de pro

**Date** : 14 mai 2026  
**Durée** : ~2-3h  
**Statut** : ✅ Complétée

---

## 🎯 Objectifs de la session

- Installer un environnement de dev complet sur Windows
- Comprendre les concepts de Git et GitHub
- Créer le repo du projet et faire le premier commit

---

## ✅ Ce qui a été fait

### Installations
- [x] Git for Windows (avec Git Bash, line endings auto, branche par défaut `main`)
- [x] VSCode + extensions C# Dev Kit et GitLens
- [x] Compte GitHub créé (username : taaaayz)
- [x] 2FA activée + recovery codes sauvegardés

### Configuration
- [x] `git config --global user.name`
- [x] `git config --global user.email` (corrigé après une erreur initiale)
- [x] `git config --global init.defaultBranch main`

### Repo
- [x] Création du repo `one-piece-rp` sur GitHub (public, MIT license, .gitignore Visual Studio)
- [x] Clone en local dans `~/Code/one-piece-rp`
- [x] Projet ouvert dans VSCode

---

## 📚 Concepts vus

### Git vs GitHub
- **Git** = outil local de versioning (sur mon ordi)
- **GitHub** = plateforme en ligne d'hébergement de repos Git

### Cycle de vie d'un fichier dans Git
- **Working Directory** : tes fichiers normaux
- **Staging** : zone tampon, ce qui va être commit
- **Committed** : sauvegardé dans l'historique Git
- **Push** : envoyé sur GitHub

### Commandes apprises
| Commande | Rôle |
|---|---|
| `pwd` | Affiche le dossier courant |
| `ls` | Liste les fichiers du dossier courant |
| `cd <dossier>` | Entre dans un dossier |
| `cd ..` | Remonte au dossier parent |
| `mkdir -p <nom>` | Crée un dossier (et ses parents si besoin) |
| `git --version` | Affiche la version de Git |
| `git config --global user.name "..."` | Définit le nom global |
| `git config --global --list` | Affiche la config globale |
| `git clone <url>` | Clone un repo distant en local |
| `code .` | Ouvre VSCode dans le dossier courant |

### Concept "Single Source of Truth"
Chaque info du projet a UN SEUL endroit officiel où elle vit.

---

## 🐛 Difficultés rencontrées

- Email mal renseigné lors du `git config user.email` → corrigé en retapant la commande (Git écrase les anciennes valeurs)
- Perte de repère après le `git clone` → confusion entre "où je suis" dans le terminal et "où est mon repo"
  - **Solution** : `pwd` pour se situer, `ls` pour voir autour, `cd` pour entrer

---

## ❓ Questions ouvertes / à creuser

- Comprendre la différence entre les branches `main` et autres (vu mais à approfondir plus tard)
- Comprendre les Pull Requests (pour quand on travaillera vraiment à plusieurs)

---

## ⏭️ Prochaine session (Session 02)

**Avant la session 02**, faire :
- [ ] Installer s&box via Steam (gros téléchargement, autant le lancer)
- [ ] Lire la doc s&box "Getting Started" si motivé

**Objectif Session 02** :
- Cadrer le GDD (Game Design Document)
- Rédiger pitch + core loop + 3 personnages MVP + système de combat chiffré
- Premier `commit` propre du GDD finalisé
