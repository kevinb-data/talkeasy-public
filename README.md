# talkeasy-public

Les pages publiques de l'application **TalkEasy**, publiées par GitHub Pages.

- `index.html` — la politique de confidentialité, celle dont l'URL est donnée à
  App Store Connect et que l'application référence dans ses mentions.

URL publique : https://kevinb-data.github.io/talkeasy-public/

## Mettre à jour

Modifier `index.html`, puis :

    git add -A && git commit -m "…" && git push

La page en ligne est rafraîchie par GitHub Pages en une minute environ.

Le texte doit rester d'accord avec ce que l'app affiche dans ses propres mentions
(`constants/talkeasy-mentions.ts` du dépôt `talkeasy`, et la ligne
`mentions.confidentialite.texte` de la table `textes` chez Supabase).
