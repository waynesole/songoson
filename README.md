# Site SonGoson · songoson.fr

Site vitrine du groupe SonGoson (musique latine et cubaine).
Il est en ligne sur **https://songoson.fr** et hébergé gratuitement par GitHub Pages.

## Comment ça marche

- Tout le site tient dans **un seul fichier** : `index.html` (textes, mise en page, couleurs).
- Les photos sont dans le dossier `img/`.
- Chaque modification enregistrée sur la branche `main` est mise en ligne automatiquement en 1 à 2 minutes.
  Si on ne voit pas le changement, il suffit de recharger la page.

## Modifier le site sur github.com (sans rien installer)

1. Ouvrir `index.html`, cliquer sur le crayon (« Edit »).
2. Chercher le texte à changer avec Ctrl+F (Cmd+F sur Mac), le modifier.
3. Cliquer sur **Commit changes** : c'est en ligne 1 à 2 minutes après.

Pour **changer une photo** : dans `img/`, faire « Add file → Upload files » avec la nouvelle photo,
puis dans `index.html` remplacer l'ancien nom de fichier (par exemple `img/hero-collage.jpg`) par le nouveau.
Mieux vaut une photo de moins de 500 Ko (largeur 1200 px suffit).

## Modifier le site avec Claude

Donner à Claude l'accès au dépôt `waynesole/songoson` et lui demander la modification en français.
Ce guide lui suffit pour s'y retrouver.

## Ce qu'il y a dans la page, dans l'ordre

| Section | Repère dans `index.html` | Contenu |
|---|---|---|
| Barre du haut | `<header class="nav">` | Logo (`img/logo.png`), liens, bouton « Demander un devis » |
| Accueil | `<section class="hero">` | Titre, texte de présentation, boutons « Voir en vidéo » puis « Réserver le groupe », photo `img/hero-collage.jpg` |
| Bandeau défilant | `<div class="marquee">` | Salsa, son cubano, Bachata… |
| Répertoire | `id="repertoire"` | 3 photos (bassiste, conguero, trompettiste) et le texte |
| Formules | `id="formations"` | Intimiste, Groupe, Formation complète |
| Où on joue | `id="evenements"` | 6 types d'événements et 3 points forts |
| Vidéos | `id="live"` | 2 liens YouTube Shorts avec leur photo |
| Devis | `id="devis"` | Téléphone, e-mail, formulaire (il ouvre la messagerie avec un e-mail pré-rempli) |
| Bas de page | `<footer>` et `<div class="mbar">` | Logo, liens, et sur téléphone les boutons « Appeler » / « Devis gratuit » |

## Coordonnées affichées

- Téléphone : **06 14 14 92 06**. Il apparaît 4 fois : le texte, le bouton « Copier » (`data-copy`),
  le lien `tel:+33614149206` dans la section Devis et le bouton « Appeler » en bas sur téléphone.
  Pour le changer, remplacer partout `06 14 14 92 06` et `+33614149206`.
- E-mail : **songoson4@gmail.com**, dans la section Devis et dans le formulaire (le script en bas de page).

## Couleurs et polices

Elles sont définies en haut de `index.html`, dans le bloc `:root` :
`--night` (fond bleu nuit), `--mango` (orange), `--rojo` (rouge du G du logo), `--cream` (texte).
Polices Google Fonts : Bricolage Grotesque (titres), Instrument Serif (italiques), Figtree (texte).

## À ne pas toucher

- Le fichier `CNAME` : il relie le site à l'adresse songoson.fr. Le supprimer coupe le domaine.
- Le haut du fichier `index.html` jusqu'à `<title>` : il contient l'aperçu affiché quand on partage le lien.

## Domaine

Le domaine `songoson.fr` est enregistré chez IONOS. Ses DNS pointent vers GitHub Pages (4 enregistrements A en 185.199.108–111.153 et un CNAME `www` vers `waynesole.github.io`).
Le certificat HTTPS est géré et renouvelé automatiquement par GitHub.
