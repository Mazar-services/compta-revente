# Compta Revente

Appli de compta pour l'achat-revente (PS5, consoles, Pokémon…) : stock avec photos et réfs, ventes, bénéfice par mois, simulateur d'achat, statistiques.

- Appli en ligne : https://mazar-services.github.io/compta-revente/
- Ce dépôt ne contient que le code. Les données sont dans le dépôt **privé** `compta-revente-donnees` (fichier `data/compta.json` + dossier `photos/`).
- Modifier l'appli ne touche jamais aux données.

## Structure

- `index.html` : toute l'appli (HTML, CSS, JS, sans dépendance ni build).
- `manifest.webmanifest`, `icon-*.png` : installation sur l'écran d'accueil.

L'appli lit et écrit `data/compta.json` via l'API GitHub avec un jeton à accès limité (Contents read/write sur le seul dépôt de données), gardé dans le navigateur de l'appareil.
