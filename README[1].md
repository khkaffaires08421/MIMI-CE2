# Mimi · Exercices CE2

Application éducative progressive pour le CE2, adaptée au mobile et à l'ordinateur.

## Contenu
- `index.html` : application et banque de questions
- `manifest.json` : installation PWA
- `service-worker.js` : cache hors connexion
- `icons/` : icônes 192 et 512 px

## Publication GitHub Pages
1. Créer un dépôt GitHub, par exemple `mimi-exercices-ce2`.
2. Téléverser tous les fichiers et le dossier `icons` à la racine.
3. Dans Settings → Pages, choisir `Deploy from a branch`, branche `main`, dossier `/ (root)`.
4. Ouvrir l'adresse GitHub Pages en HTTPS. Installer depuis le menu du navigateur.
5. Pour actualiser une version, changer `CACHE_NAME` dans `service-worker.js` (ex. `mimi-ce2-v2`).

## Google Play Store
GitHub Pages ne publie pas directement sur Play Store. Il faut convertir la PWA en application Android (de préférence Trusted Web Activity avec Bubblewrap ou PWABuilder), générer un fichier `.aab`, puis le déposer dans Google Play Console. Un compte développeur Google Play, les informations légales, la fiche de l'application et les tests exigés par Google sont nécessaires.

## Données
Les étoiles existantes restent stockées sous `localStorage` avec la clé `mimi-ce2`. Les statistiques détaillées sont ajoutées sous `mimi-ce2-stats-v1`. Ne pas effacer les données du navigateur si l'on souhaite conserver les résultats.
