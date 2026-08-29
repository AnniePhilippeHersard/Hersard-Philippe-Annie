# Site Hersard Philippe et Annie — mode d'emploi (GitHub Pages)

## Contenu du dossier
- `index.html` — le site complet (CSS, logo et illustrations intégrés).
- `mentions-legales.html` — la page mentions légales.
- `politique-confidentialite.html` — la politique de confidentialité (RGPD, Mailchimp).
- `og-image.jpg` — l'image de partage (réseaux sociaux, à partir du logo).
- `logo-hersard.svg` — le logo en vecteur (sert aussi de favicon).
- `assets/fonts/` — les polices (Fraunces, EB Garamond, Pinyon Script) intégrées au site.
- `robots.txt` et `sitemap.xml` — pour les moteurs de recherche (déjà réglés sur hersard.com).
- `README.md` — ce guide.

Pour voir le site avant publication : ouvre simplement `index.html` dans ton navigateur.

## Bon à savoir
Toutes les images sont des illustrations dessinées, intégrées au fichier. Un **portail de vérification d'âge** s'affiche à la première visite ; le choix est mémorisé sur l'appareil du visiteur.

---

## 1. Mettre en ligne sur GitHub Pages (avec GitHub Desktop)
1. Sur github.com, crée un dépôt (Repository), par exemple `site-hersard`. Coche « Public ».
2. Dans GitHub Desktop : *File → Clone repository*, choisis ce dépôt.
3. Copie tous les fichiers de ce dossier (y compris le dossier `assets/` en entier) dans le dossier du dépôt.
4. Dans GitHub Desktop : écris un résumé (« Première version »), clique **Commit**, puis **Push origin**.
5. Sur github.com, dans le dépôt : *Settings → Pages*. Sous « Branch », choisis `main` puis `/root`, et **Save**.
6. Patiente 1 à 2 minutes : l'adresse `https://ton-compte.github.io/site-hersard/` s'affiche.

## 2. Brancher ton domaine hersard.com
1. Crée un fichier nommé `CNAME` (sans extension) contenant une seule ligne : `hersard.com`.
2. Ajoute-le au dépôt (Commit + Push).
3. Chez IONOS (où le domaine est enregistré), va dans la gestion DNS de `hersard.com` et ajoute les enregistrements indiqués par GitHub dans *Settings → Pages* (des enregistrements de type A vers les adresses IP de GitHub Pages, plus un CNAME pour le sous-domaine `www` si tu le souhaites). GitHub affiche ces valeurs exactes une fois le domaine renseigné dans les réglages.
4. De retour dans *Settings → Pages*, coche **Enforce HTTPS** dès qu'elle est disponible (peut prendre jusqu'à 24h après le changement DNS).

## 3. Vérifier
Ouvre `https://hersard.com` : le portail d'âge doit s'afficher, puis le site après validation. Teste aussi `https://hersard.com/mentions-legales.html`.

---

## 4. Connecter la newsletter à Mailchimp
Voir la section dédiée ci-dessous.

## 5. Modifier un texte ou un prix plus tard
Ouvre `index.html`, modifie le texte, enregistre, puis Commit + Push dans GitHub Desktop. Aucun outil technique nécessaire.

---

## Informations légales déjà intégrées
- Éditeur : EARL Hersard Philippe, exploitation viticole « Hersard Philippe et Annie »
- SIRET : 419 784 392 00013 (SIREN 419 784 392) — Code NAF 01.21Z
- Responsable de la publication : Laurie Hersard
- Adresse : 22 et 34 rue le Bas Chelot, 37140 Saint-Nicolas-de-Bourgueil
- Téléphone : 02 47 97 48 59 — E-mail : earlhersard37@gmail.com
- Hébergeur : GitHub Pages (GitHub, Inc.)

## Options pour aller plus loin (facultatif)
- **Cloudflare** (gratuit) devant GitHub Pages si tu veux un contrôle complet des en-têtes de sécurité et un cache CDN.
