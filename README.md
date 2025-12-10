# 🏀 NBA Player Analytics Dashboard

Dashboard interactif Power BI pour l'analyse statistique approfondie des joueurs NBA.

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![NBA](https://img.shields.io/badge/NBA-253B73?style=for-the-badge&logo=nba&logoColor=white)
![Data Analysis](https://img.shields.io/badge/Data%20Analysis-4285F4?style=for-the-badge&logo=google-analytics&logoColor=white)

---

## 📋 Description du Projet

Ce projet propose un **dashboard interactif Power BI** permettant d'analyser en profondeur les performances des joueurs de la NBA. Il offre une visualisation complète et dynamique des statistiques, facilitant la comparaison entre joueurs, équipes et saisons.

Le dashboard permet aux utilisateurs de :
- 📊 Visualiser les statistiques clés des joueurs NBA (points, rebonds, passes, etc.)
- 🔍 Comparer les performances de différents joueurs
- 📈 Analyser les tendances et évolutions des performances
- ⚡ Filtrer les données par équipe, position, saison et autres critères
- 🎯 Identifier les joueurs les plus performants dans différentes catégories

---

## 🎯 Intérêts et Avantages du Dashboard

### Pour les Analystes Sportifs
- **Analyse comparative** : Comparaison rapide et visuelle entre plusieurs joueurs
- **Identification de talents** : Repérage des joueurs en progression ou sous-évalués
- **Support décisionnel** : Aide à l'évaluation des transferts et recrutements

### Pour les Fans de NBA
- **Exploration interactive** : Navigation intuitive dans les statistiques NBA
- **Débats éclairés** : Arguments factuels pour les discussions sur les meilleurs joueurs
- **Suivi de favoris** : Monitoring des performances de vos joueurs préférés

### Pour les Étudiants et Chercheurs
- **Apprentissage de Power BI** : Exemple concret de dashboard professionnel
- **Analyse de données sportives** : Cas d'étude en data analytics
- **Visualisation de données** : Bonnes pratiques de data visualization

### Avantages Techniques
- ✅ **Interface intuitive** : Pas besoin de connaissances techniques
- ✅ **Données actualisables** : Mise à jour facile des statistiques
- ✅ **Performances optimisées** : Chargement rapide et interactions fluides
- ✅ **Filtres multiples** : Exploration fine des données
- ✅ **Visualisations variées** : Graphiques adaptés à chaque type d'analyse

---

## 📁 Structure du Projet

```
NBA_dashboard_player/
│
├── README.md                          # Documentation principale
│
├── data/                              # Sources de données
│   ├── stats_par_saison.csv          # Statistiques des joueurs par saison
│   ├── head_players_placeholder.txt  # Info sur l'image d'en-tête
│   └── README.md                     # Documentation des données et API
│
├── dashboard/                         # Fichier Power BI
│   ├── NBA_Player_Dashboard.pbix     # Dashboard Power BI (à ajouter)
│   ├── README.md                     # Documentation du dashboard
│   └── .gitkeep                      # Indicateur du fichier .pbix
│
└── docs/                              # Documentation et captures
    ├── guide_utilisation.md          # Guide détaillé d'utilisation
    └── screenshots_info.md           # Information sur les screenshots
```

---

## 📊 Sources de Données

### Fichier Principal : `stats_par_saison.csv`

Les données proviennent des statistiques officielles de la **NBA saison 2023-24** et incluent :

**Statistiques par joueur** :
- 🏃‍♂️ Informations générales : Nom, équipe, position, âge, matchs joués
- ⏱️ Temps de jeu : Minutes moyennes par match
- 🎯 Statistiques offensives : Points, pourcentages de tir (FG%, 3P%, FT%)
- 🏀 Statistiques de jeu : Rebonds, passes décisives
- 🛡️ Statistiques défensives : Interceptions, contres

**Sources officielles** :
- **NBA Official Stats** : https://www.nba.com/stats/
- **NBA Stats API** : https://stats.nba.com/
- **Basketball Reference** : https://www.basketball-reference.com/

### Logos des Équipes

Les logos des équipes NBA sont récupérés via l'**API NBA officielle** :
- **Endpoint** : `https://cdn.nba.com/logos/nba/{team_id}/primary/L/logo.svg`
- **Documentation** : Voir `data/README.md` pour la liste complète des team_id

### Actualisation des Données

Les données peuvent être mises à jour facilement :
1. Télécharger les dernières statistiques depuis NBA Stats
2. Mettre à jour le fichier `stats_par_saison.csv`
3. Actualiser le dashboard dans Power BI Desktop
4. Les visualisations se mettent à jour automatiquement

---

## 🖼️ Aperçu du Dashboard

> **Note** : Les captures d'écran du dashboard doivent être ajoutées dans le dossier `docs/`

Le dashboard comprend plusieurs pages :

### Page 1 : Vue d'ensemble
- Tableau récapitulatif des joueurs
- KPI des statistiques moyennes
- Classement des meilleurs scoreurs
- Répartition par équipe

### Page 2 : Analyse comparative
- Comparaison multi-joueurs
- Radar chart des compétences
- Graphiques de performance par position

### Page 3 : Performances détaillées
- Évolution temporelle des statistiques
- Analyse des pourcentages de tir
- Corrélations entre variables
- Statistiques avancées

### Fonctionnalités Interactives
- 🔍 Filtres par équipe, position, saison, âge
- 🎯 Sélection interactive des joueurs
- 📊 Drill-down dans les données
- 🔄 Cross-filtering entre visualisations

---

## 🚀 Installation et Utilisation

### Prérequis

- **Power BI Desktop** (gratuit) : [Télécharger ici](https://powerbi.microsoft.com/fr-fr/desktop/)
- **Système d'exploitation** : Windows 10/11 ou supérieur
- **Espace disque** : ~2 GB disponible

### Étapes d'installation

1. **Cloner le dépôt**
   ```bash
   git clone https://github.com/KN13i/NBA_dashboard_player.git
   cd NBA_dashboard_player
   ```

2. **Ouvrir le dashboard**
   - Lancer Power BI Desktop
   - Fichier > Ouvrir
   - Sélectionner `dashboard/NBA_Player_Dashboard.pbix`

3. **Vérifier les sources de données**
   - Les données doivent pointer vers `data/stats_par_saison.csv`
   - Si besoin, actualiser les chemins dans Power Query

4. **Commencer l'analyse**
   - Consulter le `docs/guide_utilisation.md` pour l'aide détaillée
   - Explorer les différentes pages et filtres

---

## 📚 Documentation

- **[Guide d'utilisation complet](docs/guide_utilisation.md)** : Instructions détaillées pour utiliser le dashboard
- **[Documentation des données](data/README.md)** : Sources et structure des données
- **[Documentation dashboard](dashboard/README.md)** : Informations sur le fichier Power BI
- **[Information screenshots](docs/screenshots_info.md)** : Guide pour les captures d'écran

---

## 🔮 Améliorations Futures

### Court terme
- [ ] Ajouter des statistiques avancées (PER, True Shooting %, Usage Rate)
- [ ] Intégrer les données de plusieurs saisons pour l'analyse historique
- [ ] Créer une page dédiée aux statistiques défensives
- [ ] Ajouter des comparaisons avec les moyennes de la ligue

### Moyen terme
- [ ] Automatiser la mise à jour des données via API NBA
- [ ] Ajouter des prédictions de performance avec Machine Learning
- [ ] Créer des profils de joueurs détaillés avec photos
- [ ] Intégrer les statistiques des playoffs
- [ ] Ajouter une analyse des salaires et contrats

### Long terme
- [ ] Développer une version web du dashboard (Power BI Service)
- [ ] Créer une application mobile compagnon
- [ ] Intégrer des données de tracking (distance parcourue, vitesse)
- [ ] Ajouter l'analyse vidéo des actions clés
- [ ] Créer un système de recommandation de joueurs
- [ ] Développer des rapports automatiques personnalisés

### Améliorations Techniques
- [ ] Optimiser les performances pour de gros volumes de données
- [ ] Implémenter un système de cache pour l'API
- [ ] Ajouter des tests de qualité des données
- [ ] Créer une pipeline ETL automatisée
- [ ] Mettre en place un versioning des données

---

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. Fork le projet
2. Créer une branche pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. Commit vos changements (`git commit -m 'Add some AmazingFeature'`)
4. Push vers la branche (`git push origin feature/AmazingFeature`)
5. Ouvrir une Pull Request

---

## 📝 Licence

Ce projet est fourni à des fins éducatives et d'analyse. Les données NBA sont la propriété de la NBA.

---

## 👤 Auteur

**KN13i**

- GitHub : [@KN13i](https://github.com/KN13i)
- Projet : [NBA_dashboard_player](https://github.com/KN13i/NBA_dashboard_player)

---

## 🙏 Remerciements

- **NBA** pour les données statistiques officielles
- **Communauté Power BI** pour les bonnes pratiques et tutoriels
- Tous les contributeurs et utilisateurs du projet

---

## 📞 Support

Pour toute question ou problème :
- 🐛 Ouvrir une [issue](https://github.com/KN13i/NBA_dashboard_player/issues)
- 💬 Démarrer une [discussion](https://github.com/KN13i/NBA_dashboard_player/discussions)

---

*Dernière mise à jour : Décembre 2024*
