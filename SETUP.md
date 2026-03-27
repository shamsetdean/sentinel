# Instructions — Déploiement GitHub Pages

## Étape 1 — Créer le dépôt GitHub

1. Se connecter sur [github.com](https://github.com)
2. Cliquer sur **New repository** (bouton vert en haut à droite)
3. Nommer le dépôt : `sentinel`
4. Choisir **Public** (requis pour GitHub Pages gratuit)
5. Ne pas cocher "Initialize repository" (on va pousser les fichiers nous-mêmes)
6. Cliquer **Create repository**

---

## Étape 2 — Pousser les fichiers

```bash
# Dans le dossier sentinel-github/
cd sentinel-github

git init
git add .
git commit -m "feat: initial SENTINEL v6 landing page"

git remote add origin https://github.com/VOTRE_USERNAME/sentinel.git
git branch -M main
git push -u origin main
```

---

## Étape 3 — Activer GitHub Pages

1. Aller sur votre dépôt GitHub
2. Cliquer sur **Settings** (onglet en haut)
3. Section **Pages** (menu gauche)
4. Source : **Deploy from a branch**
5. Branch : **main** — Folder : **/ (root)**
6. Cliquer **Save**

La page sera disponible dans 1 à 3 minutes à :
```
https://VOTRE_USERNAME.github.io/sentinel/
```

---

## Étape 4 — Mettre à jour les liens de téléchargement

Dans `index.html`, remplacer les `href="#"` des boutons de téléchargement par les vraies URL des releases GitHub :

```html
<!-- Remplacer href="#" par l'URL du release -->
<a href="https://github.com/VOTRE_USERNAME/sentinel/releases/download/v6.0/SENTINEL_Intel.zip" class="version-dl">
```

Pour créer une release GitHub :
1. Onglet **Releases** sur votre dépôt
2. **Create a new release**
3. Tag : `v6.0`
4. Attacher les 4 fichiers ZIP

---

## Structure finale du dépôt

```
sentinel/
├── index.html              ← Vitrine (GitHub Pages)
├── README.md               ← Documentation
├── LICENSE                 ← Licence propriétaire SHAMS&DEAN
├── LEGAL.md                ← Mentions légales
├── PRIVACY.md              ← Politique de confidentialité
├── SETUP.md                ← Ce fichier
├── .gitignore
└── assets/
    ├── screenshot_simple.svg
    └── screenshot_expert.svg
```

---

## Domaine personnalisé (optionnel)

Pour utiliser un domaine comme `sentinel.shamsetdean.com` :

1. Dans GitHub Pages settings, saisir votre domaine
2. Créer un fichier `CNAME` à la racine :
   ```
   sentinel.shamsetdean.com
   ```
3. Configurer le DNS chez votre registrar :
   - Type CNAME : `sentinel` → `VOTRE_USERNAME.github.io`

---

*© 2025 SHAMS&DEAN*
