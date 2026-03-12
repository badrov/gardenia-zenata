# Guide de déploiement détaillé

## 🟢 Netlify (RECOMMANDÉ — 2 minutes)

1. Ouvrir https://app.netlify.com/drop dans votre navigateur
2. Glisser-déposer le fichier `index.html` dans la zone prévue
3. Attendre 30 secondes
4. Copier l'URL générée (ex: https://amazing-studio-123.netlify.app)
5. Partager cette URL partout

**Domaine personnalisé** (optionnel) :
- Dans Netlify → Site settings → Domain management
- Ajouter votre domaine (ex: studio-gardenia-zenata.com)
- Acheter le domaine sur Godaddy.com (~10€/an)

---

## 🐙 GitHub Pages (gratuit illimité)

```bash
# 1. Installer Git si nécessaire
# 2. Créer un repository sur github.com
# 3. Dans votre terminal :
git init
git add index.html
git commit -m "Studio Gardenia landing page"
git remote add origin https://github.com/VOTRE-NOM/studio-gardenia.git
git push -u origin main

# 4. Sur GitHub : Settings → Pages → Branch: main → Save
# URL : https://VOTRE-NOM.github.io/studio-gardenia
```

---

## ▲ Vercel (performances maximales)

1. https://vercel.com → Sign up (gratuit)
2. "Add New Project" → "Browse" → sélectionner le dossier
3. Deploy → URL publique en 60 secondes

---

## 📊 Tracking des visites (optionnel)

Ajoutez Google Analytics en insérant avant `</head>` :
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## 🔧 Modifications rapides

| Élément | Où modifier dans index.html |
|---------|----------------------------|
| Prix | Chercher "720 000 DH" → remplacer |
| Téléphone | Chercher "33651489658" → remplacer |
| Email | Chercher "badr.nasser@gmail.com" → remplacer |
| Loyer estimé | Chercher "3 500–4 500 DH" → remplacer |
