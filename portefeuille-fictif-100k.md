# Portefeuille fictif · objectif 100 000 €

## État courant

| Indicateur | Valeur |
|---|---:|
| Date de référence initiale (Europe/Paris) | 2026-11-20 |
| Titres (valorisations fournies) | 10 252,07 € |
| Espèces (EUR) | 1 642,11 € |
| Valeur initiale reconstituée et valeur courante de référence | 11 894,18 € |
| Total affiché par le courtier (informatif) | 11 952,61 € |
| Écart non ventilé, exclu de l'actif et du cash | 58,43 € |
| Plus-value latente historique fournie | +173,58 € (+1,72 %) |
| Performance depuis le départ simulé | 0,00 % |
| Valeur maximale observée depuis le départ simulé | 11 894,18 € |
| Apports/retraits depuis l'ouverture | 0,00 € |
| Benchmark | CW8, référence de départ 667,22 € (cours fourni) |
| Dernière exécution simulée | Aucune |

Les prix d'origine sont ceux du relevé fourni, avec valeurs arrondies. Pour l'initialisation, faire primer les valorisations en euros fournies sur le produit du prix arrondi par la quantité. Les actions américaines figurent en équivalent EUR dans le relevé. Pour les cotations suivantes, retenir par défaut la ligne US en USD, puis convertir en EUR. Les prix de revient d'origine sont indicatifs, distincts de la performance depuis l'ouverture du portefeuille fictif.

## Positions

| Instrument | Ticker, place, devise de négociation | Quantité | PRU EUR fourni | Cours EUR fourni | Valorisation EUR initiale | P/L latent historique EUR |
|---|---|---:|---:|---:|---:|---:|
| Adobe | ADBE, Nasdaq, USD | 4 | 306,96 | 202,89 | 811,58 | −416,26 |
| Albemarle | ALB, NYSE, USD | 8 | 68,62 | 74,40 | 595,23 | +46,24 |
| Alphabet A | GOOGL, Nasdaq, USD | 8 | 220,71 | 248,23 | 1 985,86 | +220,17 |
| Amazon | AMZN, Nasdaq, USD | 3 | 229,82 | 227,34 | 682,02 | −7,44 |
| Amundi MSCI World Swap UCITS ETF EUR Acc | CW8, Euronext Paris, EUR, LU1681043599 | 4 | 655,83 | 667,22 | 2 668,88 | +45,57 |
| Microsoft | MSFT, Nasdaq, USD | 3 | 338,72 | 446,94 | 1 340,81 | +324,64 |
| Nvidia | NVDA, Nasdaq, USD | 3 | 145,80 | 123,46 | 370,37 | −67,03 |
| ServiceNow | NOW, NYSE, USD | 12 | 88,20 | 82,27 | 987,19 | −71,26 |
| Shopify | SHOP, Nasdaq, USD | 7 | 101,60 | 115,73 | 810,13 | +98,95 |

## Ordres

| ID | Date de décision | Instrument | Sens | Quantité | Type | Limite | Actif à partir de | Échéance | État | Prix exécuté | Frais EUR |
|---|---|---|---|---:|---|---:|---|---|---|---:|---:|
| PF-20261120-01 | 2026-11-20 | GOOGL, Nasdaq, USD | Vente | 2 | Limite | 280,00 USD | Ouverture régulière du 2026-11-23 | Clôture régulière du 2026-11-25 | En attente | — | — |

PF-20261120-01. Alléger sur rebond pour diminuer le poids d'Alphabet d'environ 17,4 % à 13,3 % en incluant son exposition indirecte via CW8, à prix d'origine comparables. Le seuil se situe près de la clôture du 17 novembre (280,20 USD). Dans la séance du 20 novembre, 273,67 USD à 12 h 19 ET et 273,00 USD à la mi-séance selon les repères disponibles au moment de la décision. La croissance du Cloud soutient la thèse sur les six titres conservés, tandis que le free cash-flow du T3, à −9,07 milliards USD, justifie un poids moindre. Réévaluer si une nouvelle annonce significative intervient avant le déclenchement.

## Historique de portefeuille

| Date | Valeur EUR | Espèces EUR | Perf. depuis départ | Benchmark CW8 depuis départ | Statut |
|---|---:|---:|---:|---:|---|
| 2026-11-20 | 11 894,18 | 1 642,11 | 0,00 % | 0,00 % | Relevé de départ, cours fournis. Ordre de vente GOOGL posé pour la séance suivante. |

Références de l'initialisation et de la décision :

- [Alphabet T3 2026 (SEC)](https://www.sec.gov/Archives/edgar/data/1652044/000165204426000080/googexhibit991q32026.htm)
- [Cours historiques GOOGL](https://chartexchange.com/symbol/nasdaq-googl/historical/)
- [Fiche Amundi CW8 octobre 2026](https://www.amundietf.fr/pdfDocuments/monthly-factsheet/LU1681043599/FRA/FRA/RETAIL/ETF/20261031)
- [Situation de marché du 20 novembre (Benzinga, 12 h 43 ET)](https://www.benzinga.com/markets/equities/26/11/63492512/stock-market-today-nasdaq-100-nvidia-seventh-day-chipmakers-smh)

## Conventions de simulation

- Gestion fictive active, horizon principal de 1 à 6 mois. Espèces réutilisables après exécution confirmée. Sans levier, sans positions vendeuses et sans apports par défaut. Les quantités sont entières.
- Conserver un identifiant unique par ordre et un point de portefeuille par date. Les exécutions et annulations sont historisées. La modification d'une limite nécessite l'annulation de l'ancien ordre et la création d'un nouvel ordre avec un identifiant distinct.
- Simuler 1,00 € de frais par ordre effectivement exécuté. Hors fiscalité et frais de change additionnels. Convertir les flux USD au dernier taux de référence EUR/USD BCE disponible au moment du flux, par division USD/(USD par EUR). Rester cohérent avec le calendrier de disponibilité des taux. Inscrire la date du taux utilisé, les dividendes crédités et les opérations sur titres vérifiables.
- Contrôler les ordres en attente avant décision. Pour un ordre limite actif avant l'ouverture régulière, utiliser une ouverture au prix limite ou meilleur si vérifiée, sinon retenir de manière conservatrice le prix limite si le seuil a été clairement franchi après l'activation. Un ordre placé en cours de séance ne peut se fonder que sur des données horodatées postérieures à son activation. Une mèche antérieure, un simple contact intrajournalier ou une donnée ambiguë ne valent pas exécution. Si un seuil est franchi après le briefing, traiter l'exécution au point suivant, à la date à laquelle elle a eu lieu. Ne jamais décompter deux fois le même ordre.
- Publier la valeur en EUR à partir de cours et du change datés. Privilégier des clôtures comparables d'une même date disponible. Quand des cours manquent ou sont décalés, qualifier la valorisation de provisoire ou reporter le dernier point complet. Si des flux ou ordres interviennent après le point de valorisation, les dater séparément. Comparer à CW8 avec des dates de référence compatibles.

## Point de gestion — 2026-11-22 (dimanche, marchés fermés)

**Décision : CONSERVER les neuf positions. Aucun ordre nouveau, exécuté ou annulé.** L'ordre PF-20261120-01 (vente limite de 2 GOOGL à 280 USD) reste **EN ATTENTE**, activable uniquement à l'ouverture régulière du Nasdaq le 23 novembre, avec échéance le 25 novembre. Aucune transaction fictive n'a été comptabilisée, aucune commission débitée.

**État comptable confirmé (dernier instantané fourni le 20 novembre) :** titres 10 252,07 €, espèces 1 642,11 €, total 11 894,18 €, référence CW8 667,22 €. Performance cumulée depuis cet instantané : 0,00 % *par construction*, et non performance de marché. Valeur maximale observée sur les points confirmés : 11 894,18 € ; recul confirmé 0,00 % (non actualisé). Distance à 100 000 € : 88 105,82 €. Aucune valorisation comparable de clôture complète au 20 novembre n'a été établie pour les neuf lignes avec un taux EUR/USD BCE cohérent : performance quotidienne, écart CW8 et drawdown de marché **non calculables**, et aucune nouvelle ligne de valorisation chiffrée n'est créée.

**Contexte vérifié du vendredi 20 novembre :** Nasdaq -5,28 %, S&P 500 -3,70 %, Nvidia -14,01 %. La pression s'est concentrée sur l'IA et les semi-conducteurs, avec des interrogations sur la rentabilité des dépenses d'infrastructure et la trajectoire des taux. Cela augmente le risque de facteur commun entre NVDA, GOOGL, MSFT, AMZN, NOW, ADBE et l'exposition technologique indirecte via CW8. Le mouvement ne prouve pas à lui seul une révision durable des profits : aucune vente forcée ni renforcement aveugle avant d'obtenir des données comparables. Sources : [Washington Post, 20 novembre](https://www.washingtonpost.com/business/2026/11/20/us-stock-market-slumps-amid-rising-tech-ai-worries/), [StockTitan, clôture du 20 novembre](https://www.stocktitan.net/articles/stock-market-today-live-november-20-2026).

**Deux déclencheurs à surveiller lundi 23 novembre :** (1) GOOGL à 280 USD ou plus **après** activation de l'ordre ; une simple cotation non horodatée ne suffit pas pour exécuter. (2) Confirmation ou non du rebond des semi-conducteurs après la chute de NVDA de 14,01 %, et actualisation des révisions de bénéfices avant tout nouvel achat.

**Synchronisation :** point inscrit sur GitHub. La copie Library d'origine est restée à l'état du 20 novembre faute d'outil d'édition en place ; le présent point n'affecte ni quantités ni cash et doit être réconcilié à la prochaine écriture Library possible.
