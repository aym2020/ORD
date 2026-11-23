# Portefeuille fictif · objectif 100 000 €

## Dernier état comptable confirmé — non revalorisé

**Contrôle de fraîcheur du 23 novembre 2026 :** les quantités et les espèces ci-dessous sont celles du dernier état **comptablement confirmé**. Les valorisations EUR par ligne et le total de **11 894,18 €** sont toujours ceux de l'instantané d'ouverture du **20 novembre 2026**, **pas des cours actuels du 23 novembre**. Les briefings ont été ajoutés, mais aucun mark-to-market intégral des neuf positions avec taux BCE cohérent n'a été enregistré. **Valeur de marché courante : non déterminée** ; performance et écart CW8 actualisés : non déterminés. Il faut publier un nouveau point complet (ou un provisoire de séance clairement horodaté) avant de qualifier la valeur de « courante ». L'absence d'ordre exécuté ne signifie pas que la valeur des titres n'a pas changé.

## État de référence initial (20 novembre 2026)

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


## Réévaluation après ouverture US — 2026-11-23 (point précoce, vers 16 h 25–16 h 30 Europe/Paris)

**Décision : CONSERVER. Aucun nouvel ordre.** L'ordre `PF-20261120-01` (vendre 2 GOOGL à 280 USD, Nasdaq, actif depuis l'ouverture régulière du 23 novembre, échéance 25 novembre) demeure **EN ATTENTE — EXÉCUTION NON CONFIRMÉE**. La cotation GOOGL de **282,86 USD à 09:19:15 ET** du 23/11 est expressément **préouverture** ; elle ne prouve pas l'atteinte du seuil durant la séance régulière. La source Yahoo Finance consultée ne fournissait pas de prix régulier postérieur à 09:30 ET horodaté et vérifiable. Ne pas débiter 2 actions ni créditer le cash ; ne pas appliquer de frais. La prochaine réévaluation devra chercher l'ouverture régulière et les transactions horodatées après 09:30 ET avant toute exécution, puis utiliser le taux BCE disponible au moment de la transaction.

**Marché à l'ouverture :** les dépêches du 23/11 décrivent un rebond américain spectaculaire, Nasdaq environ +6,6 % et Nvidia environ +30 %, déclenché par l'annonce du retour de Jensen Huang à la tête de Nvidia. L'information soutient le sentiment IA mais ne résout pas à elle seule les questions de valorisation, de dépenses de centres de données, de gouvernance ou de contrôles à l'export. Le signal est trop corrélé aux lignes NVDA/MSFT/GOOGL/AMZN/NOW/ADBE et à CW8 pour engager de nouveaux achats à l'ouverture sans vérifier les cours de chaque ligne et la tenue du rebond.

**État comptable confirmé inchangé :** 8 GOOGL et les huit autres lignes initiales ; espèces **1 642,11 €**, titres au dernier relevé fourni **10 252,07 €**, total de référence **11 894,18 €** au 20/11. Distance à 100 000 € **88 105,82 €**. Performance du 23/11, écart à CW8 et drawdown actualisé **non calculables** sans neuf cotations cohérentes, CW8 et change daté. Ne pas présenter le total de référence comme une valorisation de séance. Aucun mouvement de trésorerie confirmé.

**Deux niveaux/événements à surveiller :** (1) prix d'ouverture et transactions régulières GOOGL à 280 USD ou plus, puis validation de l'ordre `PF-20261120-01` selon le protocole ; (2) maintien du rebond NVDA/semiconducteurs après la première heure et ses implications sur les révisions de bénéfices.

**Sources consultées le 23/11 :** [Yahoo Finance GOOGL, préouverture 09:19:15 ET à 282,86 USD](https://finance.yahoo.com/quote/GOOGL/history/), [Investors.com, couverture de l'ouverture US](https://www.investors.com/market-trend/stock-market-today/dow-jones-sp500-nasdaq-nvidia-nvda-crowdstrike-zscaler/), [BCE, taux EUR/USD de référence (dernier affiché le 20/11 : 1,0990)](https://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/eurofxref-graph-usd.cs.html).

**Réconciliation :** journal Library inchangé au 20/11 ; GitHub conserve aussi le point du 22/11. Aucun ordre ou flux n'a été ajouté dans cette réévaluation ; les registres CSV restent inchangés et cohérents. Le briefing du matin du 23/11 n'était pas présent sur GitHub au moment du contrôle.
