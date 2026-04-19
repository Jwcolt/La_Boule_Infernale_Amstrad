# La_Boule_Infernale_Amstrad
reproduction du jeu la Boule Infernale de 1985 sur Amstrad CPC
more work to be done to go back to this amazing game from 1985 that I spent hours on it.

# 🎮 La Boule Infernale

> Remake fidèle du jeu publié dans le magazine **Hebdogiciel** pour **Amstrad CPC** — années 85.

![Amstrad CPC](https://img.shields.io/badge/Amstrad-CPC-yellow) ![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange) ![Langue](https://img.shields.io/badge/Langue-Français-blue) ![License](https://img.shields.io/badge/License-MIT-green)

---

## 🕹️ Jouer

Télécharge `index.html` et ouvre-le dans n'importe quel navigateur moderne (Chrome, Safari, Firefox).  
Aucune installation, aucune dépendance.

Ou joue directement en ligne via **GitHub Pages** :  
👉 `https://TON_USERNAME.github.io/boule-infernale/`

---

## 📖 Histoire

La Boule Infernale est un jeu d'adresse publié dans les années 80 dans le magazine français **Hebdogiciel**, sous forme de listing à taper soi-même sur Amstrad CPC. Ce remake en HTML5/Canvas reproduit fidèlement l'esthétique et le gameplay de l'original : fond noir, bordure damier jaune, sprites pixel-art, et sons rétro générés par Web Audio API.

---

## 🎯 Objectif

Collecter les **10 clefs jaunes** dispersées sur l'écran sans percuter les **blocs verts** (murs).  
Une seule vie. Pas de second essai.

---

## 📋 Règles

| Élément | Comportement |
|---|---|
| 🟡 **Boule** | Se déplace horizontalement en continu |
| 🔑 **Clef jaune** (×10) | À collecter — +1 point, la boule repart en sens inverse |
| 🟩 **Bloc vert** (×10) | Mur à éviter — collision = game over immédiat |
| 🏁 **Niveau suivant** | Les 10 clefs collectées → nouveau terrain généré aléatoirement |
| 💀 **Game over** | 1 seule vie — tout recommence |

---

## 🎮 Contrôles

| Touche | Action |
|---|---|
| `ESPACE` | Démarrer / lancer la boule |
| `↑` (maintenu) | Dévier la boule vers le haut |
| `↓` (maintenu) | Dévier la boule vers le bas |
| Relâcher `↑` ou `↓` | Retour au mouvement horizontal pur |

> **Logique rétro :** la boule va de gauche à droite par défaut. Le joueur ne fait que dévier sa trajectoire verticalement pendant l'appui. Dès que la touche est relâchée, la boule reprend son cap horizontal.

---

## 🏆 Tableau des scores

- **Top 10** sauvegardé localement (localStorage)
- Classement : **score décroissant** → en cas d'égalité, **temps croissant**
- Si tu entres dans le top 10 : saisie de ton nom + `ENTRÉE` pour valider
- Podium avec médailles ① ② ③

---

## 🔊 Sons

Sons rétro générés par **Web Audio API** — aucun fichier audio externe :

| Événement | Son |
|---|---|
| Rebond sur bord | Bip square wave descendant |
| Collecte d'une clef | Arpège ascendant 3 notes |
| Collision mur (mort) | Descente sawtooth |
| Passage de niveau | Fanfare 4 notes |

---

## ⚙️ Technique

- **Langage** : HTML5 / JavaScript vanilla
- **Rendu** : Canvas 2D (800×520px)
- **Audio** : Web Audio API (aucune dépendance)
- **Stockage** : localStorage pour le tableau des scores
- **Compatibilité** : Chrome, Safari, Firefox, Edge — aucun serveur requis

---

## 📁 Structure

```
boule-infernale/
├── index.html   ← Le jeu complet (fichier unique)
└── README.md    ← Ce fichier
```

---

## 👤 Auteur

Remake réalisé par **Jean-Michel Colnot**  
Inspiré du listing original paru dans **Hebdogiciel** (années 80)

---

## 📜 Licence

MIT — libre d'utilisation, de modification et de distribution.
