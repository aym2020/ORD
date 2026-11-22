# ORD — Portefeuille fictif vers 100 000 €

Gestion active **100 % fictive**, en EUR, depuis le 20 novembre 2026 : capital initial de **11 894,18 €** (titres : 10 252,07 € ; espèces : 1 642,11 €). Écart inexpliqué de 58,43 € exclu.

## Organisation

- [Journal de référence](portefeuille-fictif-100k.md) : quantités, cash, historique et conventions de calcul.
- [Instructions permanentes](AGENTS.md) : mandat détaillé et règle de décision.
- [Protocole](docs/PROTOCOLE.md) : vérification, traçabilité et synchronisation.
- [Briefings](briefings/) : points de gestion datés, y compris incidents.
- [Ordres](registre/ordres.csv) : carnet des ordres fictifs, identifiants uniques.
- [Valorisations](registre/valorisations.csv) : dates de cours, cash, performance et benchmark.

La tâche ChatGPT est configurée pour publier quotidiennement son analyse et consigner les changements sur la branche principale. Les commits **ne sont pas des exécutions de courtier** : aucun ordre réel n'est passé. Les opérations fictives restent en attente sans preuve d'une transaction simulée selon les conventions.

Pour chaque séance, rapprocher **GitHub et le journal Library** `libfile_b0e72a5fc1cc819191fe69687216d712` ; ne jamais écraser un état plus récent ni inventer de cours. En cas d'indisponibilité GitHub, publier le briefing et journaliser précisément le défaut de synchronisation.

> Ce dépôt est actuellement public. Ne jamais y déposer de données personnelles, secrets ou identifiants.
