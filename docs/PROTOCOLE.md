# Protocole de gestion quotidienne

1. **Lecture avant toute décision.** Lire la dernière version du journal GitHub et du journal Library `libfile_b0e72a5fc1cc819191fe69687216d712`. Réconcilier les différences : les deux états peuvent avoir des écritures non synchronisées. Faire primer les mouvements vérifiés ; ne jamais revenir à un ancien état sans contrôle.
2. **Ordres existants.** Contrôler l'activation et l'échéance de chaque ordre. Ne valider une exécution qu'à partir de cours datés *postérieurs* à l'activation. Éviter les doubles réservations de titres et de cash. Les ordres sont exclusivement simulés.
3. **Analyse.** Examiner les publications, surprises vs consensus, réactions des cours, informations sectorielles, macroéconomiques, réglementaires, géopolitiques et leurs impacts sur résultats, marges, cash-flow, taux et valorisations. Comparer les alternatives en 1–6 mois et les expositions communes via les ETF.
4. **Décision.** Conserver, acheter, renforcer, alléger ou vendre ; produire pour tout nouvel ordre un ID unique, quantité, ticker, place, devise, type, limite/seuil, activation, échéance et justification. Pour les achats : objectif, invalidation, horizon et risque de gap significatif.
5. **Comptabilité.** Réconcilier positions et espèces ; frais de 1,00 € par ordre exécuté ; dernier EUR/USD de référence BCE disponible au moment du flux ; dividendes et opérations sur titres seulement si vérifiés. Ajouter chaque mouvement une seule fois.
6. **Valorisation.** Utiliser des cours homogènes et datés en EUR. Qualifier les valorisations provisoires, distinguer instantané initial et clôtures comparables. Reporter le cash, P/L depuis le départ, performance du jour si calculable, CW8, écart relatif, drawdown depuis le plus haut et distance aux 100 000 €.
6 bis. **Mark-to-market obligatoire.** À chaque passage, essayer de mettre à jour la valorisation de TOUTES les lignes, avec un cours horodaté par titre, la conversion BCE applicable, le cash réconcilié et la référence CW8. Au briefing du matin, utiliser les dernières clôtures comparables. À 16 h 30, un instantané intraday est PROVISOIRE et doit indiquer ses horodatages ; ne pas le confondre avec une clôture américaine. Mettre à jour le tableau de positions et `registre/valorisations.csv` même en l'absence d'ordre si la valeur évolue et peut être établie. Une ligne de valorisation doit être unique par date **et type de point** (matin/après-ouverture/clôture). Si le marché ou le change est insuffisamment vérifiable, indiquer la dernière valeur complète avec sa **date réelle** et un statut `NON_ACTUALISE`, expliciter les cours manquants, et ne pas afficher la valeur du 20/11 comme actuelle. Ne jamais inventer un chiffre pour remplir le registre.
7. **Commit et continuité.** Mettre à jour le journal complet, les deux registres CSV et un briefing `briefings/YYYY-MM-DD.md`. Vérifier les SHA avant écriture sur GitHub et après. Mettre à jour Library dans la mesure du possible. En cas d'indisponibilité d'un système, conserver un état sûr et afficher explicitement le blocage dans le briefing.
8. **Week-end/jour férié.** Faire un point court des nouvelles et préparer la réouverture ; ne pas inventer d'exécutions pendant les fermetures.
9. **Vie privée.** Ce dépôt GitHub est public. N'y déposer ni secrets, ni informations privées ni données de courtier réel.

## Présentation et écriture du tableau de bord

Le fichier `portefeuille-fictif-100k.md` est un **tableau de bord Markdown GitHub**, **pas** un journal de briefings. À **chaque** exécution (9 h et 16 h 30), même sans opération, vérifier sa fraîcheur et **réécrire sa synthèse** en conservant toutes les positions et le cash, sans y ajouter de paragraphes narratifs. Respecter la structure : **statut + date des cours → KPI → progression vers 100 000 € → tableau complet des positions trié par poids → ordres en tableau → deux déclencheurs → liens vers briefings et registres**. Les métriques non établies apparaissent en `N/D`, pas comme des 0 % ou comme d'anciennes valeurs présentées comme actuelles. Une donnée initiale conserve toujours sa date du 20/11/2026.

Écrire l'**analyse exhaustive** uniquement dans `briefings/YYYY-MM-DD.md`, avec les sources et les décisions. Mettre l'historique des ordres dans `registre/ordres.csv` et les points de valorisation uniques (par date et type de point) dans `registre/valorisations.csv`. Git conserve les anciennes versions du tableau de bord. **Interdiction de recopier les briefings dans le tableau de bord.**

Avant le commit, contrôler : total des positions + cash = total portefeuille si valorisation possible ; toutes les quantités et l'ordre actif apparaissent ; les cours sont datés ; dernière date de valorisation explicitement affichée ; le tableau de bord est toujours lisible sans dérouler de « pavés de texte ». Écrire et vérifier les commits de la vue portefeuille et du briefing. Ne pas retarder la publication visible en cas d'indisponibilité d'une source.

## Historique initial

Le 20/11/2026, valeur de référence issue du relevé utilisateur : 11 894,18 € (10 252,07 € de titres et 1 642,11 € d'espèces), écart non attribué de 58,43 € exclu. Ordre `PF-20261120-01` : vente limite de 2 GOOGL à 280 USD, activation le 23/11/2026, échéance le 25/11/2026 ; en attente avant l'ouverture du 23/11. Le 21/11/2026, le système de tâches a fonctionné sans livrer de briefing ; aucune transaction simulée vérifiée.

Le code d'un commit atteste seulement l'enregistrement d'un document ; il n'atteste pas l'exécution boursière.

## Contrôle de fin d'exécution — critères vérifiables (incident 26/11/2026)

À chaque analyse automatique, la réponse ChatGPT n'est **pas** le livrable unique : le travail reste partiel tant que les écritures durables n'ont pas été **tentées puis vérifiées**. Exécuter la séquence dans cet ordre :

1. Lire les sources GitHub et Library dans l'ordre prescrit ; vérifier le dernier ordre et la cohérence des quantités et du cash.
2. Tenter les neuf cours cohérents et le change BCE. Si les cours manquent, **continuer quand même** à l'étape suivante avec `NON_ACTUALISE` et le dernier point complet daté. Jamais de prix fabriqué.
3. **Écrire réellement** le briefing daté et réécrire `portefeuille-fictif-100k.md` à **chaque** passage. Si une valeur complète est calculée, ajouter une ligne unique au CSV des valorisations ; ne jamais doubler un ordre.
4. **Relire** le briefing, le tableau de bord et le CSV concerné sur GitHub après les écritures ; vérifier leurs contenus et le SHA du dernier commit. Une intention d'écrire n'est pas une preuve.
5. **Remplacer** la même copie Library `libfile_b0e72a5fc1cc819191fe69687216d712` avec le tableau de bord GitHub réellement committé, puis vérifier que les contenus sont concordants (une normalisation du saut de ligne final est acceptable). Ne jamais recopier un état Library plus ancien sur GitHub.
6. Publier dans ChatGPT : verdict, ordres, valorisation datée, cash, performance, CW8, drawdown, distance à l'objectif, deux déclencheurs, statut des deux écritures GitHub et de la Library, **lien du commit vérifié**. Signaler toute anomalie persistante avec l'étape échouée et le message d'erreur.

**Règle anti-faux succès :** si une écriture attendue n'a pas abouti, l'analyse demeure *PARTIELLE* même si le texte a été envoyé et même si le planificateur indique « completed ». Si les outils d'écriture sont indisponibles, l'indiquer exactement, sans inventer une panne GitHub. Une fermeture de marché ne dispense ni de la valorisation aux dernières clôtures complètes ni des écritures.

## Revue de l'univers investissable — contrôle stratégique obligatoire

La tâche quotidienne combine **(1) tenue des positions et sécurité comptable** et **(2) sélection active d'investissements hors portefeuille**. L'une ne remplace jamais l'autre. Dans le briefing daté, ajouter après le point comptable une section `Recherche hors portefeuille et concurrence du capital` contenant :

- **Couverture réellement effectuée** : marchés, secteurs, nombre et/ou familles d'actions effectivement vérifiés, dates et sources (univers indicatif : top 50 US, leaders européens, midcaps US/Europe liquides ; l'univers ne doit pas être limité aux neuf lignes).
- **Au moins trois dossiers externes évalués au matin** ou signalement explicite des données manquantes : catalyseur, dernier fait vs consensus, situation fondamentale, sensibilité des résultats, cours et valorisation datés, scénario 1–6 mois, déclencheur et invalidation. Au point après-ouverture, réévaluer la shortlist et chercher les nouvelles surprises de la séance.
- **Classement comparatif** des idées externes et détenues, incluant le cash. Identifier la ligne éventuellement finançable et expliciter pourquoi l'ordre est préférable à `CONSERVER`. Ne pas obliger un ordre par jour : l'activité est la **recherche**, pas la rotation pour la rotation.
- **Verdict opérationnel** : `ACHETER / ALLEGER / VENDRE / RENFORCER / ATTENDRE` pour chaque action proposée et conditions de déclenchement. Sans cours ou valorisation fiable : `SURVEILLER — pas d'ordre`, sans cible inventée.

Dans chaque briefing quotidien, préciser `Couverture externe : FAITE / PARTIELLE / NON FAITE`, indépendamment de `Synchronisation technique : OK / PARTIELLE`. Une réussite GitHub/Library ne valide **jamais** à elle seule une bonne analyse d'investissement. Toute comparaison chiffrée et toute anticipation doivent citer leur source avec date. Tenir compte des précédents sans biais rétrospectif.

## Résolution des références Library après remplacement

Après remplacement, relister le dossier `/ORD` sur la surface Library, retrouver l'entrée par son identifiant Library permanent, puis lire avec le `file_id` courant ou la nouvelle référence de résultat de listing. Ne pas réutiliser une référence de lecture antérieure au remplacement. Comparer le texte intégral au tableau GitHub relu (normalisation du saut final admise). En cas d'erreur de visibilité, relister avant de réessayer. Pour la couverture stratégique, consigner les titres réellement examinés et les sources consultées, distinguer balayage initial et shortlist approfondie ; rechercher les cours manquants par une seconde source indépendante avant de conclure N/D. Ne pas déclarer une couverture complète sans preuve.
