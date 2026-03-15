# LevéO Academy — Landing Page

Landing page statique pour [leveo.academy](https://leveo.academy).
Hébergée sur GitHub Pages. Formulaire via Web3Forms. Zéro backend, zéro framework.

---

## Déploiement

### Étape 1 — Web3Forms (2 min)

1. Aller sur [web3forms.com](https://web3forms.com)
2. Entrer l'email : `adrien@leveo.academy`
3. Recevoir la clé API par email
4. Dans `index.html`, remplacer `REMPLACER_PAR_TA_CLE_WEB3FORMS` par la clé reçue
5. Commit & push le changement

### Étape 2 — GitHub Pages

1. Aller dans **Settings > Pages**
2. Source : **Deploy from branch** > `main` > `/ (root)`
3. Custom domain : `leveo.academy`
4. Cocher **Enforce HTTPS**

### Étape 3 — DNS (OVH)

Dans la zone DNS de `leveo.academy`, supprimer les enregistrements A existants puis créer :

| Type   | Nom  | Valeur                  |
|--------|------|-------------------------|
| A      | @    | 185.199.108.153         |
| A      | @    | 185.199.109.153         |
| A      | @    | 185.199.110.153         |
| A      | @    | 185.199.111.153         |
| CNAME  | www  | `<TON-USERNAME>.github.io` |

Propagation DNS : 15 à 60 minutes.

---

## Structure

```
index.html   ← tout le site (HTML + CSS + JS)
CNAME        ← domaine custom pour GitHub Pages
README.md    ← ce fichier
```

---

## Stack

- HTML / CSS / JS vanilla
- Google Fonts (Outfit)
- Web3Forms (formulaire)
- GitHub Pages (hébergement)
