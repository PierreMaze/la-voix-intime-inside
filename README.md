# "INSIDE" — Le Trésor des 9 Portes

Page d’inscription responsive en React, Vite et Tailwind CSS v4.

## Démarrer

```sh
npm install
npm run dev
```

## Production

```sh
npm run build
npm run preview
```

Les fichiers à héberger sont générés dans `dist/`.

Le lien PayPal est défini par `PAYPAL_URL` dans `src/main.jsx`. Les boutons ouvrent ce lien sans collecter de données bancaires sur la page. Le paiement fractionné dépend de l’éligibilité déterminée par PayPal. Aucune confirmation de paiement automatique n’est implémentée.

Les deux visuels fournis sont dans `public/images/`. Le format vertical est utilisé sur les petits mobiles, le format horizontal sur les écrans plus larges. Les polices DM Sans et Manrope sont chargées depuis Google Fonts, avec repli sans-serif.


## Publication GitHub Pages

Site public : https://PierreMaze.github.io/la-voix-intime-inside/

Dépôt : https://github.com/PierreMaze/la-voix-intime-inside

Après une modification, enregistrer et pousser les sources avec Git, puis lancer :

```sh
npm run deploy
```

Cette commande compile le site puis publie `dist/` sur la branche `gh-pages`. GitHub Pages utilise cette branche, dossier racine. Un simple push des sources ne republie pas la page : relancer `npm run deploy` pour mettre le site à jour.

La base `/la-voix-intime-inside/` est définie dans `vite.config.js`. Les images utilisent `import.meta.env.BASE_URL` pour fonctionner sous cette adresse. L’aperçu local est accessible sous ce même chemin.
