# PWA Lecture GPS, version de test

Contenu du dossier, à déposer tel quel à la racine d'un dépôt GitHub :
- `index.html` : la page élève (76 exercices, autonomie et guidé), autonome, avec la déclaration PWA ;
- `manifest.webmanifest` : nom, couleurs, icônes (installation sur l'écran d'accueil) ;
- `sw.js` : service worker (fonctionnement hors ligne après la première visite) ;
- `icons/` : icônes 192, 512, maskable et icône Apple ;
- `.nojekyll` : empêche GitHub Pages de retraiter les fichiers.

## Mise en ligne (GitHub Pages)
1. Créer un dépôt, par exemple `QCM-GPS-test`, public (GitHub Pages gratuit).
2. Déposer tout le contenu de ce dossier à la racine (GitHub Desktop ou « Add file > Upload files », sans oublier `.nojekyll`).
3. Settings > Pages > Source : branche `main`, dossier `/ (root)`.
4. Adresse obtenue au bout d'une minute : `https://victors2i.github.io/QCM-GPS-test/`.

## Installation côté élève
- Android (Chrome) : menu ⋮ puis « Installer l'application » ou « Ajouter à l'écran d'accueil ».
- iPhone (Safari) : bouton Partager puis « Sur l'écran d'accueil ».

## Mise à jour
Remplacer `index.html` dans le dépôt, puis changer `VERSION` dans `sw.js` (par exemple `gps-v2`). Le service worker charge d'abord la version en ligne, donc la nouvelle page apparaît à l'ouverture suivante avec du réseau.

## Remarques
- Fichier d'environ 8 Mo : le premier chargement est un peu long en 4G, ensuite tout est en cache.
- La progression éventuelle est stockée dans le navigateur de chaque élève (pas de serveur).
- Contrôles faits en local : service worker actif, mise en cache complète, page affichée hors ligne, aucune erreur JavaScript.
