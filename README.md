# Studio aux Glovettes – site vitrine

Site d'une seule page (`index.html`), sans dépendance, hébergé gratuitement sur GitHub Pages.

- Dépôt : `auxGlovettes/site-studio`
- Adresse du site : https://auxglovettes.fr (domaine défini dans le fichier `CNAME`, ne pas le supprimer)
- Annonce : https://www.airbnb.fr/h/foxyglovy (page française) et https://www.airbnb.com/h/foxyglovy (page anglaise)
- Contact : contact@auxglovettes.fr (lien `mailto:` dans la section Réserver et dans les mentions légales des deux pages)

## Contenu du dépôt

| Fichier | Rôle |
|---|---|
| `index.html` | Page en français (texte, styles, mise en page) |
| `en/index.html` | Même page en anglais, accessible sur `/en/` |
| `photos/` | Photos du studio, partagées par les deux langues |
| `CNAME` | Nom de domaine personnalisé pour GitHub Pages |

## Photos

Les photos sont dans le dossier `photos/` (JPEG, 1 200 px de large, issues de l'annonce Airbnb) :

| Fichier | Utilisation |
|---|---|
| `hero.jpg` | Image d'en-tête et aperçu lors d'un partage du lien |
| `sejour.jpg` | Galerie : séjour et lit double |
| `alcove.jpg` | Galerie : alcôve et lit double |
| `cabine.jpg`, `cabine-2.jpg` | Galerie : coin cabine, lits superposés et entrée |
| `repas.jpg` | Galerie : coin repas |
| `cuisine.jpg` | Galerie : cuisine |
| `sdb-baignoire.jpg`, `sdb-lavabo.jpg`, `sdb-rangements.jpg` | Galerie : salle de bain (baignoire, lavabo et lave-linge, rangements) |
| `balcon-2.jpg`, `balcon.jpg` | Galerie : balcon |
| `vue.jpg`, `vue-hiver.jpg` | Galerie : vue en été et en hiver |

Pour changer une photo, remplacer le fichier en gardant le même nom (JPEG, 1 600 px de large maximum). Pour en ajouter une, la déposer dans `photos/` puis ajouter une ligne `<figure>` dans la galerie de `index.html`.

## Langues

Le site existe en français (`index.html`) et en anglais (`en/index.html`). Un sélecteur **FR | EN** en haut à droite de la barre de navigation permet de passer de l'une à l'autre. Les deux pages déclarent leurs équivalents (`hreflang`) pour le référencement.

Toute modification de contenu (texte, prix, équipements, photos) doit être faite **dans les deux fichiers**. Les photos, elles, sont communes : remplacer un fichier de `photos/` met à jour les deux langues.

## Publication

Le site est publié par GitHub Pages depuis la branche `main` (Settings → Pages → Deploy from a branch → `main` / `(root)`). Chaque `git push` sur `main` met le site à jour en 1 à 2 minutes.

## Modifier le site

- Petite retouche : ouvrir `index.html` (et `en/index.html`) sur GitHub, cliquer sur le crayon, puis « Commit ». Le site se met à jour tout seul.
- Avec Claude Code : ouvrir le dossier du dépôt, demander la modification dans les deux langues, vérifier le résultat dans un navigateur, puis `git push`. Pour tester le changement de langue en local, il faut un petit serveur (par exemple `npx serve`), car les liens `/en/` ne fonctionnent pas en ouvrant directement le fichier.

## À faire plus tard

- Ajouter les étoiles de classement et le numéro d'enregistrement en mairie, une fois obtenus.
