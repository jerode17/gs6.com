Voici un README prêt à ajouter au dépôt — je l’ai préparé en français pour expliquer le projet, l’usage et le déploiement.

````markdown name=README.md
# GS6 — Landing & QR

Une landing page simple et un générateur de QR codes pour la marque GS6.

## Contenu du dépôt
- `index.html` — page de destination responsive + générateur de QR (client‑side). Permet :
  - saisir l'URL de destination,
  - uploader un logo (optionnel) pour l'insérer au centre du QR,
  - choisir couleur, taille et niveau de correction d'erreur,
  - télécharger le QR en SVG ou PNG.
- `CNAME` — contient `GS6.com` (permet de lier le domaine au site GitHub Pages).

## Utilisation rapide
1. Tester localement : ouvrir `index.html` dans un navigateur.
2. Générer un QR :
   - saisir l'URL (par défaut `https://GS6.com`),
   - uploader le logo (optionnel),
   - choisir taille/couleur/niveau d'erreur (`H` recommandé si logo central),
   - cliquer sur "Générer le QR" puis télécharger en SVG ou PNG.
3. Fichiers imprimables : préférer le SVG pour l'impression. Fournir PNG 600–1200 px si nécessaire.

## Déploiement sur GitHub Pages
1. Pousser `index.html` et `CNAME` sur la branche `main`.
2. Dans le dépôt → Settings → Pages → Source : choisir `main` / `root`, puis Save.
3. Attendre que GitHub publie le site (quelques minutes). L'URL publique s'affichera dans la section Pages.

## Connexion du domaine (GS6.com)
Pour connecter l'apex (GS6.com) chez votre registrar, ajoutez les A records suivants :
- 185.199.108.153
- 185.199.109.153
- 185.199.110.153
- 185.199.111.153

Conserver le fichier `CNAME` dans le repo ; GitHub émettra automatiquement le certificat HTTPS (délai : quelques minutes à quelques heures).

## Conseils pour l'impression des QR
- Utiliser le SVG (vectoriel) pour un rendu net à toute échelle.
- Taille imprimée recommandée pour étiquette : ≥ 4 cm de côté (augmenter pour lecture à distance).
- Si vous placez un logo au centre : utiliser correction d'erreur `H` (30%) et garder le logo ≤ 20–25% de la taille du QR.
- Tester le QR avec plusieurs téléphones avant impression massive.

## Licence & droits
Contenu et visuels : propriété de GS6. Ajoutez une licence (ex. MIT) si vous souhaitez autoriser la réutilisation publique.

## Besoin d'aide
Si tu veux que je pousse ces fichiers pour toi et active Pages, donne le lien du dépôt et confirme que l'invitation collaborateur est acceptée. Je peux aussi générer et fournir ici des SVG/PNG de haute résolution du QR pour impression.
````
