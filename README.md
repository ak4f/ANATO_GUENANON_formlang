# Formlang — Bibliothèque Théorie des Langages

**Projet Réalisé par le Binôme 5 :**
- ANATO K. Freddy
- GUENANON K. C. Ulysse

**Documentation détaillée :** [Lien vers le rapport (PDF)](docs/RAPPORT.pdf)

## Présentation du Projet
`formlang` est une bibliothèque Python 3 unifiée implémentant la hiérarchie de Chomsky de manière ascendante. Elle offre un cœur algorithmique robuste et modulaire (automates, grammaires, machines de Turing) utilisé par plusieurs applications concrètes :

- **Morpho** : Analyseur morphologique (BUTA).
- **Shield** : Détecteur d'attaques par LLM (double encodage) via des automates d'arbres.
- **Hashcons** : Optimisation mémoire de la création d'arbres syntaxiques (DAG).
- **MTU** : Calculatrice basée sur des Machines de Turing Universelles.

## Installation & Exécution

L'ensemble des composants a été couvert par des tests unitaires (`pytest`).

```bash
# Lancer l'intégralité des 28 tests unitaires
pytest -q

# Lancer la démonstration complète (Pipeline Shield, Morpho, MTU)
python pipeline.py
```

## Architecture
L'architecture de `formlang` repose sur un principe strict de séparation : les dossiers `apps/` (logique métier) se contentent d'**instancier** les objets mathématiques définis dans `formlang/` (le cœur théorique).

---
*Projet réalisé dans le cadre du module Théorie des Langages et Automates.*
