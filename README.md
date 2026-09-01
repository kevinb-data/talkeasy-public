# talkeasy-public

Le site public de l'application **TalkEasy**, publié par GitHub Pages sur le nom de domaine
**[talkeasy-app.fr](https://talkeasy-app.fr/)**.

| Fichier                | Adresse                                      | Ce que c'est |
| ---------------------- | -------------------------------------------- | ------------ |
| `index.html`           | https://talkeasy-app.fr/                     | La vitrine : l'icône, une phrase, le bouton App Store |
| `confidentialite.html` | https://talkeasy-app.fr/confidentialite.html | La politique de confidentialité, dont l'URL est donnée à App Store Connect |
| `support.html`         | https://talkeasy-app.fr/support.html         | L'assistance, dont l'URL est donnée à App Store Connect |
| `assets/`              | —                                            | Les images de la vitrine, fabriquées depuis celles de l'app |
| `CNAME`                | —                                            | Le fichier qui branche le domaine. **Ne pas le supprimer.** |

Chaque page porte sa propre feuille de style, recopiée plutôt que partagée : aucune dépendance
entre elles, donc une ligne cassée ne peut pas en emporter deux autres. Les trois se répondent par
des liens en pied de page.

## Mettre à jour

Modifier le fichier, puis :

    git add -A && git commit -m "…" && git push

La page en ligne est rafraîchie par GitHub Pages en une minute environ.

## Ce qui doit rester d'accord

- **La confidentialité se dit à trois endroits** : cette page, la doublure de
  `constants/talkeasy-mentions.ts` dans le dépôt `talkeasy`, et la ligne
  `mentions.confidentialite.texte` de la table `textes` chez Supabase. Changer ce que l'app fait,
  c'est changer les trois.
- **L'assistance est seule à dire ce qu'elle dit** : ce qui en est recopié dans l'app n'est que le
  filet de trois phrases qui monte si le téléphone refusait d'ouvrir une adresse. Les quatre
  questions et leurs réponses se corrigent donc ici, sans toucher à l'app.
- **Les adresses vivent aussi dans l'app**, dans `ADRESSES` de `constants/talkeasy-mentions.ts`.
  Renommer un fichier ici, c'est corriger cette ligne-là, puis la fiche App Store, puis
  reconstruire l'app.
