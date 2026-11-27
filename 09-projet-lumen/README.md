# Projet Lumen : intégrer l'IA dans une équipe, de A à Z

> **Cas fictif** construit pour la formation : l'entreprise Lumen Distribution, les personnes et les chiffres sont inventés. Les situations sont inspirées de cas fréquents.

Sophie Marchal dirige le service client de Lumen Distribution (180 salariés, matériel électrique pour les professionnels) : 14 conseillers, 600 demandes par semaine, 26 heures de délai moyen de première réponse. Son directeur lui dit : « Il faut faire quelque chose avec l'IA. » Deux conseillers utilisent déjà un assistant gratuit, sans le dire.

Ce dossier suit son projet étape par étape, avec tous les documents qu'elle a produits. Chaque étape correspond à une partie de la formation.

| Étape | Partie de la formation | Document |
|---|---|---|
| 1. Le point de départ | Ouverture | [01-point-de-depart.md](01-point-de-depart.md) |
| 2. La carte des usages | Partie 2, atelier 1 | [02-carte-des-usages.md](02-carte-des-usages.md) |
| 3. L'analyse de l'usage prioritaire | Partie 3, atelier 2 | [03-grille-d-analyse.md](03-grille-d-analyse.md) |
| 4. Le cadre juridique | Partie 4 | [04-cadre-juridique.md](04-cadre-juridique.md) |
| 5. L'essai et le baromètre | Intersession | [05-experimentation.md](05-experimentation.md) |
| 6. La réunion de lancement | Parties 5 et 6, atelier 3 | [06-lancement.md](06-lancement.md) |
| 7. La sécurité au quotidien | Partie 7 | [07-securite.md](07-securite.md) |
| 8. La charte, puis l'assistant | Partie 8, atelier 4 | [08-charte.md](08-charte.md) · [assistant/](assistant/) |
| 9. Le bilan à 90 jours | Clôture | [09-bilan-90-jours.md](09-bilan-90-jours.md) |

Le registre des usages de l'équipe : [registre-des-usages.md](registre-des-usages.md).

## L'assistant de l'équipe

```
assistant/
├── CLAUDE.md            les instructions (instructions) : rôle, règles, interdits
├── AGENTS.md            le même contenu, pour les outils qui lisent ce nom de fichier
├── MEMORY.md            la mémoire (memory) : conventions apprises, relue chaque mois
├── garde-fous.md        les garde-fous (guardrails) : cinq niveaux, demande à la DSI
├── connaissances/       les connaissances (knowledge) : réponses de référence, délais
└── competences/         les compétences (skills) : une procédure par dossier
    ├── retard-livraison/SKILL.md
    ├── retour-produit/SKILL.md
    └── compte-rendu-appel/SKILL.md
```
