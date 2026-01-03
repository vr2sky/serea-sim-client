# SEREA — Simulation Client

Ce dépôt est un **client externe de démonstration** pour le SaaS **SEREA**.

Il illustre comment un tiers (ex. GitHub Actions) peut appeler l’API
`/saas/v1/decision/simulate` afin d’obtenir une **décision de gouvernance**
(ALLOW / DENY) **sans effet de bord**.

## Ce que ce dépôt est
- Un **consommateur** de l’API SEREA
- Une **simulation réaliste** d’usage client
- Un support de démonstration et de validation produit

## Ce que ce dépôt n’est pas
- ❌ Le code de SEREA
- ❌ Une intégration CI/CD de production
- ❌ Un composant interne du produit

## Principe
- Authentification via token SaaS (secret GitHub Actions)
- Appel de l’endpoint de simulation
- Résultat exploitable (logs + artefact JSON)

## Sécurité
Aucun secret n’est stocké dans le dépôt.
Les credentials sont fournis via **GitHub Actions secrets**.
