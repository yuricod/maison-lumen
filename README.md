# Maison Lumen · Analyse commerciale

**702 326 € de chiffre d’affaires TTC en 2025, en hausse de 6,7 % sur un an.** Cette étude académique suit les ventes d’une enseigne fictive de janvier 2023 à décembre 2025. Elle examine aussi la répartition des offres personnalisées entre les groupes de clientèle.

[Ouvrir le tableau de bord dans Google Colab](https://colab.research.google.com/github/yuricod/maison-lumen/blob/main/05_dashboard_plotly.ipynb)

## Trois décisions à éclairer

| Question | Résultat observé | Piste d’action |
|---|---|---|
| Quand préparer les stocks ? | Décembre présente le coefficient saisonnier le plus élevé (1,46), août le plus faible (0,70). | Anticiper le pic de décembre et comparer les ventes aux mêmes mois de l’année précédente. |
| Quels canaux suivre ? | Le magasin représente 49,4 % du CA sur trois ans. L’application apporte la plus forte contribution positive à la croissance entre 2024 et 2025, environ 26 767 €. | Suivre les commandes et le panier moyen de chaque canal pour comprendre la progression. |
| Les offres atteignent-elles les groupes d’âge de façon comparable ? | L’écart entre les taux extrêmes passe de 31,8 à 30,9 points après la refonte. | Examiner le ciblage à canal comparable. L’analyse porte sur les commandes observées et ne couvre pas les personnes qui n’ont rien acheté. |

## Données et méthode

Les fichiers sources contiennent 24 224 lignes. Après retrait de 121 doublons exacts puis de 14 avoirs négatifs, l’analyse conserve **24 089 commandes**. Le CA additionne les montants TTC après remise sur ce périmètre. Les remboursements exclus seraient à réintégrer pour un rapprochement comptable. La comparaison avant et après la refonte décrit une évolution sans établir son origine.

## Parcourir les notebooks

1. [Explorer les données et vérifier le nettoyage](01_exploration_autonome.ipynb)
2. [Comparer les canaux et les segments de clientèle](02_univarie_bivarie.ipynb)
3. [Mesurer la tendance et la saisonnalité des ventes](03_series_temporelles.ipynb)
4. [Examiner les écarts de ciblage avec Fairlearn](04_biais_fairlearn.ipynb)
5. [Consulter les indicateurs et exporter le tableau de bord Plotly](05_dashboard_plotly.ipynb)

## Reproduire le tableau de bord

Ouvrir le dernier notebook dans Colab, dans une session neuve, puis choisir **Exécution → Tout exécuter**. La première cellule installe Fairlearn et télécharge la configuration pédagogique depuis Google Drive. Le chargement des données nécessite une connexion et dépend de la disponibilité des ressources du cours. Garder le secteur `commerce`. La dernière cellule génère et télécharge `dashboard_commerce.html`, consultable ensuite dans un navigateur.

Les résultats présentés ici proviennent des sorties enregistrées dans les notebooks.
