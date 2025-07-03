# EXERCICE: Affichage d'un message de succès

## 🎯 Objectifs de l’exercice

On veut afficher un message de succès temporaire — comme sur un vrai site web — qui disparaît **progressivement** après 3 secondes. Pour cela, on utilise `setTimeout()` et une **transition CSS** sur l’opacité.

## 🎨 Instructions CSS

Dans le fichier `style.css`, modifiez ou créez la classe `.success-msg` pour qu'elle:

- [ ] ait une `transition` de **1 seconde sur l’opacité**.
- [ ] ait une opacité initiale de `1`.

De plus,

- [ ] ajoutez aussi une classe `.fade-out`
- [ ] appliquez-lui une opacité de `0`.

> 💡 La transition entre `.success-msg` et `.fade-out` rendra l’effet fluide.

## 💻 Instructions JavaScript

Lorsque l’on clique sur le bouton `"Clique-moi"` ci-bas (le bouton rouge):

- [ ] Créez un **nouveau paragraphe (`<p>`)** contenant le texte `"Bravo!"`
- [ ] Ajoutez ce paragraphe **dans le `<div>` ayant la classe `.container`**
- [ ] Appliquez à ce paragraphe :
  - [ ] une couleur de fond verte `rgb(0, 128, 0)`,
  - [ ] la classe `.success-msg`
  - [ ] une opacité initiale de `1` (peut être via CSS ou JS)
- [ ] **Après 3 secondes**, ajoutez-lui la classe `.fade-out` (il commencera à disparaître). Utilisez la méthode `setTimeout()` pour cela.
- [ ] **Lorsque la transition est terminée**, supprimez le paragraphe du DOM

> 💡 Il existe un événement nommé `transitionend` qui est activé lorsque la transition CSS est terminée.