# TD Swagger — API Bibliothèque HEI

Spécification OpenAPI 3.0 (OAS3) d'une API de gestion de bibliothèque, construite de façon incrémentale au fil des exercices du TD.

## Description

Chaque fichier YAML représente une étape de conception de l'API `API Bibliotheque HEI`, qui gère les livres et les emprunts. La spécification part d'un squelette vide et s'enrichit progressivement jusqu'à un CRUD complet.

## Progression des exercices

| Fichier | Contenu |
|---------|---------|
| `ex01_*.yaml` | Squelette OpenAPI (`info`, `paths` vide) |
| `ex02_*.yaml` | Ajout d'un premier endpoint |
| `ex03_*.yaml` | `GET /livres/{id}` avec paramètre de chemin |
| `ex04_*.yaml` | Réponse `404` sur `GET /livres/{id}` |
| `ex05_*.yaml` | Pagination (`page`, `limit`) sur `GET /livres` |
| `ex06_*.yaml` | `POST /livres` avec `requestBody` et réponses `201`/`422` |
| `ex07_*.yaml` | Enrichissement des schémas et réponses |
| `ex08_*.yaml` | CRUD complet : `PUT`, `PATCH`, `DELETE` sur `/livres/{id}` |

> Les fichiers sont nommés `exNN_std_25_001_std_25_027.yaml` (numéro d'étape + identifiants des étudiants).

## Endpoints (version finale)

- `GET /livres` — Lister les livres (pagination `page`, `limit`)
- `POST /livres` — Créer un livre
- `GET /livres/{id}` — Lire un livre
- `PUT /livres/{id}` — Remplacer un livre
- `PATCH /livres/{id}` — Modifier un livre
- `DELETE /livres/{id}` — Supprimer un livre

## Utilisation

Ouvrir n'importe quel fichier `.yaml` dans [Swagger Editor](https://editor.swagger.io/) pour visualiser et tester la spécification.
