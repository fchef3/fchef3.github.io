# Mon blog de sécurité offensive

Jekyll + thème Chirpy, déployé sur GitHub Pages.

## Mise en ligne

1. Crée un dépôt GitHub **public** nommé `TON_USER_GITHUB.github.io`.
2. Dézippe cette archive, puis dans le dossier :
   ```bash
   git init -b main
   git add .
   git commit -m "Initial commit"
   git remote add origin git@github.com:TON_USER_GITHUB/TON_USER_GITHUB.github.io.git
   git push -u origin main
   ```
3. Sur GitHub : *Settings → Pages → Build and deployment → Source : GitHub Actions*.
4. Le workflow `pages-deploy.yml` construit et publie le site à chaque push.

## À personnaliser (cherche `TON_` et `TODO`)

- `_config.yml` : titre, tagline, pseudo, liens, URL
- `_tabs/about.md` : ta présentation
- `_data/contact.yml` : icônes de contact
- Avatar : dépose une image dans `assets/img/` puis renseigne `avatar:` dans `_config.yml`

## Écrire un article

Copie `_drafts/TEMPLATE-writeup.md` vers `_posts/AAAA-MM-JJ-titre.md`, puis modifie l'en-tête.

## Tester en local

```bash
bundle install
bundle exec jekyll serve   # http://127.0.0.1:4000
# avec les brouillons : bundle exec jekyll serve --drafts
```

## Avant de publier un article

- [ ] Aucune IP, domaine, jeton ou identifiant réel
- [ ] Métadonnées EXIF retirées des captures
- [ ] Cible autorisée ou plateforme d'entraînement
- [ ] Pas de flag d'une épreuve encore active
