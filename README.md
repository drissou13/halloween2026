# 🕸️ Le Manoir Hanté — notice à lire avant d'entrer

> *Vous tenez entre vos mains le grimoire d'un site que peu ont osé publier.
> Lisez-le en entier avant de frapper à la porte. On ne vous aura pas prévenu deux fois.*

---

## 🎃 Ce que renferme ce fichier

Un seul parchemin : `halloween.html`.
Pas de dépendances à invoquer, pas d'installation rituelle — HTML, CSS et JavaScript dorment tous les trois dans le même cercueil.

À l'intérieur du manoir :

- une grille d'entrée qui reste **verrouillée toute l'année**, sauf une nuit
- un décompte macabre jusqu'à l'ouverture
- la légende du manoir, à lire à voix basse
- une porte sur laquelle on peut frapper — la troisième fois n'est jamais anodine
- trois citrouilles à ouvrir, entre friandise et mauvaise surprise
- une ambiance sonore que vous devrez activer vous-même (rien ne hurle sans votre accord)

---

## 🔒 Le sortilège de verrouillage

Le manoir ne s'ouvre que le **31 octobre**, selon l'horloge de celui qui pousse la grille.
Le reste de l'année, seul un portail scellé apparaît, avec son propre compte à rebours.

Le reste du site n'est pas simplement *caché* derrière un voile — il n'est tout bonnement pas révélé tant que la date n'est pas la bonne.

**Pour forcer l'ouverture avant l'heure** (utile si vous êtes le gardien du manoir et non un simple visiteur), ajoutez ceci à la fin de l'adresse :

```
?preview=halloween
```

Ce passe-droit n'est écrit nulle part sur la façade. Vous seul(e) le connaissez, désormais.

---

## 🦇 Comment invoquer le site

Trois façons de faire tourner la clé dans la serrure :

1. **Ouverture directe** — double-cliquez sur `halloween.html`. Tout navigateur moderne s'en accommodera.
2. **Sur un serveur local**, si vous préférez que le rituel soit plus solennel :
   ```bash
   python3 -m http.server 8000
   ```
   puis rendez-vous sur `http://localhost:8000/halloween.html`.
3. **En ligne** — déposez le fichier sur l'hébergeur de votre choix (Netlify, GitHub Pages, ou tout autre cimetière numérique). Aucune base de données, aucune clé API : le fichier se suffit à lui-même.

---

## 🕯️ Personnaliser le grimoire sans se brûler les doigts

| Vous voulez... | Cherchez dans le fichier... |
|---|---|
| Changer la date d'ouverture | la fonction `nextHalloween()` dans le `<script>` de bas de page |
| Réécrire la légende du manoir | la section `<section class="legend">` |
| Changer les couleurs (sang, os, brume) | les variables tout en haut du `<style>`, sous `:root` |
| Ajouter une quatrième citrouille | dupliquez une ligne `<button class="pumpkin">` et une entrée dans le tableau `outcomes` du script |
| Adoucir ou intensifier le cri | la fonction `playShriek()` |

---

## ⚰️ Compatibilité

Fonctionne sur ordinateur comme sur mobile, de jour comme — surtout — de nuit.
Respecte les préférences d'accessibilité : si le visiteur a demandé moins d'animations à son appareil, les battements de chauve-souris et le sursaut de la porte s'apaisent d'eux-mêmes.

---

*Ce fichier s'autodétruira dans votre mémoire dans... non, en fait, gardez-le. Vous en aurez besoin l'année prochaine.*
