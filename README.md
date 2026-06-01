# Imoria — Documentation

Source publique de la documentation Imoria, hébergée sur Mintlify.

**Site live** : à configurer dans Mintlify dashboard.

## Stack

- Mintlify (Free tier) — auto-deploy via GitHub
- Contenu MDX français, voix impersonnelle / 3e personne
- Branding Imoria — accent `#e43416` vermillon (OKLch token `oklch(60% 0.215 32)` du design system Imoria)
- Police Inter (sans, body + heading)

## Structure

```
docs.json                 # Mintlify config (theme, nav, branding)
index.mdx                 # Landing — Qu'est-ce qu'Imoria
demarrer/                 # Installation + premier prompt
chercher/                 # Recherche par critères / sémantique / sous-cotées / inspecter
evaluer/                  # Estimation / comparables / quartier / marché
geo/                      # Géocodage + filtre POI
ressources/               # Limites, FAQ, glossaire, référence outils
```

## Règles éditoriales

- **Voix** : français impersonnel / 3e personne ("Imoria + verbe", infinitifs, "on"). Jamais "tu" ni "vous".
- **Mentions interdites** : "Leboncoin", "LBC". Toujours "annonces particulières et professionnelles".
- **Pas de documentation** : authentification, tokens, quotas, scopes — gérés hors de la doc publique.
- **Pas d'AI slop** : références Linear / Stripe / Bloomberg, pas Anthropic Discord blob. Pas d'emoji.
- **Couverture Alsace-Moselle** : signaler explicitement le gap DVF pour les dépts 57, 67, 68 avec `<Warning>`.

## Workflow

1. Édition locale ou via PR sur ce repo.
2. Push vers `main` → Mintlify auto-deploy en ~30 sec.
3. Preview de PR auto-générée par Mintlify sur chaque branche.

Source de vérité produit : [`iFeyz/goldsky-lbc` — spec docs v1](https://github.com/iFeyz/goldsky-lbc/blob/main/docs/superpowers/specs/2026-06-01-imoria-gitbook-docs-v1-design.md) (légacy GitBook, contenu identique).
