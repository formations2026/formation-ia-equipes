# Les garde-fous (guardrails) de l'assistant Lumen

Aucun garde-fou ne suffit seul. Une règle écrite dans CLAUDE.md oriente l'assistant mais ne l'empêche pas techniquement d'agir : tout ce qui serait grave doit être rendu impossible par la technique.

## Les cinq niveaux

| Niveau | Ce qui est en place à Lumen | Responsable |
|---|---|---|
| 1. Les règles écrites (instructions) | CLAUDE.md : rôle, interdits, phrases de refus | Sophie et l'équipe |
| 2. Les droits d'accès (permissions) | L'assistant lit les connaissances ; il ne peut ni envoyer de courriel, ni accéder au logiciel de facturation, ni modifier une commande | DSI |
| 3. Les filtres (filters) | Les IBAN et numéros de carte sont détectés et masqués avant traitement | DSI |
| 4. La validation humaine (human-in-the-loop) | Chaque brouillon est relu et envoyé par un conseiller | Équipe |
| 5. La traçabilité (logging) et la revue | Conversations conservées 30 jours ; revue mensuelle des erreurs ; relecture mensuelle de la mémoire | Comité IA, Inès |

## De la charte aux garde-fous

| Règle de la charte | Instruction (niveau 1) | Phrase de refus | Garde-fou technique |
|---|---|---|---|
| Rien ne part sans relecture | Tu produis uniquement des brouillons | — | Aucun droit d'envoi (niveau 2) |
| Pas de donnée bancaire | Refuse tout RIB ou IBAN | « Donnée rouge : retire-la avant de continuer. » | Filtre IBAN (niveau 3) |
| Pas de délai inventé | Délais uniquement depuis connaissances/ | « Délai à confirmer. » | Accès limité à la base validée (niveau 2) |
| Pas de geste commercial | Ne propose ni remise ni remboursement | « Je le signale à votre conseiller. » | Validation humaine (niveau 4) |
| Transparence | Termine par « Brouillon IA, à relire. » | — | Journal des brouillons (niveau 5) |

## Ce que Sophie a demandé à la DSI (par écrit)

1. Aucun droit d'envoi de courriel, de modification de commande ou d'accès à la facturation pour l'assistant.
2. Un filtre sur les données bancaires en entrée.
3. Un accès limité au dossier connaissances/, en lecture seule.
4. La conservation des conversations pendant 30 jours, puis suppression.
5. La possibilité, pour l'équipe, de lire et de corriger la mémoire de l'assistant.
