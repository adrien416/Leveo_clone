# LevéO — Page de redirection

LevéO a fermé ses portes. Ce dépôt héberge désormais une simple **page de redirection**
qui envoie les visiteurs de `leveo.academy` vers **[Prouesse](https://prouesse.vc)**.

## Fonctionnement

- `index.html` : page de clôture aux couleurs de LevéO, avec redirection automatique
  vers `https://prouesse.vc` après 6 secondes (compte à rebours + bouton manuel).
- Redirection assurée par `<meta http-equiv="refresh">` (fallback sans JS) et par JavaScript.

## Hébergement

Le site est hébergé sur **Netlify**, connecté au domaine `leveo.academy` (OVH).

## Redirection instantanée (optionnel)

Pour une redirection immédiate côté serveur (sans afficher la page), ajouter un fichier
`_redirects` à la racine avec :

```
/*  https://prouesse.vc  301
```

Netlify appliquera alors une redirection permanente 301 avant même d'afficher la page.
