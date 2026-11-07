# Planning du restaurant

**👉 Ouvrir l’application en ligne : https://maxime3738.github.io/planning-restaurant/**

Application de planning pour les salariés du restaurant : créneaux par jour, total d’heures par semaine et par mois, comparaison avec le contrat. Tout tient dans un seul fichier : `index.html`.

## Ouvrir l’application sur l’ordinateur

Double-cliquez sur `index.html`. Il s’ouvre dans votre navigateur (Chrome, Edge, Firefox ou Safari). Rien à installer, aucune connexion Internet nécessaire.

Au premier lancement, 5 salariés fictifs et une semaine d’exemple sont chargés. Le bouton **Tout effacer** (en bas de la page) permet de repartir de zéro.

## Mettre l’application en ligne gratuitement

Une fois en ligne, l’application s’ouvre avec un simple lien, sur ordinateur comme sur téléphone.

### Option 1 : Netlify Drop (le plus simple, 2 minutes)

1. Créez un dossier (par exemple `planning`) et mettez-y `index.html`.
2. Allez sur **https://app.netlify.com/drop**.
3. Glissez-déposez **le dossier** dans la zone prévue.
4. Netlify affiche un lien du type `https://nom-au-hasard.netlify.app` : c’est votre application.
5. Connectez-vous ou créez un compte Netlify gratuit quand c’est proposé : c’est ce qui garde le site en ligne durablement. Vous pouvez ensuite renommer le lien (Site configuration → Change site name).

Pour publier une nouvelle version : dans Netlify, ouvrez le site → onglet **Deploys** → glissez de nouveau le dossier.

### Option 2 : GitHub Pages

1. Créez un compte gratuit sur **https://github.com**.
2. Cliquez sur **+** (en haut à droite) → **New repository**. Donnez-lui un nom (par exemple `planning`), cochez **Public**, puis **Create repository**.
3. Sur la page du dépôt, cliquez sur **uploading an existing file**, glissez `index.html` (et `README.md` si vous voulez), puis **Commit changes**.
4. Allez dans **Settings** → **Pages**. Sous « Branch », choisissez **main** et le dossier **/ (root)**, puis **Save**.
5. Attendez 1 à 2 minutes. Le lien apparaît en haut de la page Pages : `https://votre-nom.github.io/planning/`.

Pour publier une nouvelle version, ré-uploadez `index.html` dans le dépôt.

> Mettre une nouvelle version en ligne ne touche pas à vos données : elles restent dans votre navigateur.

## Sauvegarder et restaurer les données

Chaque modification est **enregistrée automatiquement** dans le navigateur : pas de bouton « Sauvegarder ». L’heure du dernier enregistrement s’affiche sous le titre.

- **Exporter** : télécharge un fichier de sauvegarde, par exemple `planning-restaurant-2026-11-07.json`. Gardez-le en lieu sûr (clé USB, Google Drive, e-mail…).
- **Importer** : choisissez un fichier exporté. L’application vous demande de confirmer avant de **remplacer** les données actuelles.
- Un rappel discret apparaît si aucun export n’a été fait depuis plus de 7 jours.
- Le bouton **Annuler** (ou Ctrl+Z) revient sur la dernière modification, tant que la page reste ouverte.

Pour passer à un autre appareil ou un autre navigateur : **Exporter** sur l’ancien, puis **Importer** sur le nouveau.

## ⚠️ Important : où sont stockées les données ?

Les données sont enregistrées **dans le navigateur utilisé, sur l’appareil utilisé**. Concrètement :

- un seul appareil et un seul navigateur : le planning saisi sur l’ordinateur n’apparaît pas sur le téléphone (et inversement) ;
- le fichier ouvert en local (double-clic) et la version en ligne ont chacun **leurs propres données** ;
- vider les données de navigation (cookies et données de sites) ou utiliser la navigation privée **efface** le planning ;
- si le navigateur bloque l’enregistrement, un bandeau rouge s’affiche en haut de la page.

Exportez donc une sauvegarde régulièrement.

## Mode d’emploi rapide

- **Case du planning** : touchez-la pour ajouter, modifier ou supprimer des créneaux, ou pour marquer Repos, Congé, Absent ou Maladie. Un créneau qui passe minuit (ex. 18:00 → 01:00) est accepté. Il compte en entier pour le jour où il commence.
- **En-tête d’un jour** : copier toute la journée vers d’autres jours, ou la vider.
- **Copier vers la semaine suivante** : duplique la semaine affichée.
- **Vue Mois** : heures de chaque semaine et total du mois. « Base contrat » = contrat hebdomadaire × jours du mois ÷ 7.
- **Couleurs** : vert = contrat respecté, orange = heures manquantes, rouge = dépassement. La tolérance se règle dans **Salariés → Réglages**.
- **Imprimer / PDF** : imprime la vue affichée en A4 paysage. Choisissez « Enregistrer en PDF » comme imprimante pour obtenir un PDF.
- **Mode sombre** : bouton lune / soleil en haut à droite (mémorisé).
