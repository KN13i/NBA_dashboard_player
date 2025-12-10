# Guide d'utilisation - Dashboard NBA Player Analytics

## Table des matières
1. [Installation et Ouverture](#installation-et-ouverture)
2. [Navigation dans le Dashboard](#navigation-dans-le-dashboard)
3. [Utilisation des Filtres](#utilisation-des-filtres)
4. [Interprétation des Visualisations](#interprétation-des-visualisations)
5. [Astuces et Conseils](#astuces-et-conseils)

---

## Installation et Ouverture

### Étape 1 : Installer Power BI Desktop
1. Téléchargez Power BI Desktop depuis le site officiel : https://powerbi.microsoft.com/fr-fr/desktop/
2. Installez l'application en suivant les instructions à l'écran
3. Lancez Power BI Desktop

### Étape 2 : Ouvrir le Dashboard
1. Cliquez sur **Fichier** > **Ouvrir**
2. Naviguez vers le dossier `dashboard/`
3. Sélectionnez le fichier `NBA_Player_Dashboard.pbix`
4. Le dashboard s'ouvre et charge les données

---

## Navigation dans le Dashboard

### Pages disponibles

Le dashboard contient plusieurs pages accessibles via les onglets en bas :

#### 🏀 Page 1 : Vue d'ensemble
- **Description** : Vue générale des statistiques des joueurs NBA
- **Contenu** :
  - Tableau récapitulatif des meilleurs joueurs
  - KPI (indicateurs clés) : Moyenne de points, rebonds, passes
  - Classement des équipes
  - Top scoreurs de la saison

#### 📊 Page 2 : Analyse comparative
- **Description** : Comparez les performances de différents joueurs
- **Contenu** :
  - Graphiques de comparaison multi-joueurs
  - Radar chart des compétences
  - Analyse par position
  - Statistiques avancées

#### 📈 Page 3 : Performances détaillées
- **Description** : Analyse approfondie des statistiques individuelles
- **Contenu** :
  - Évolution des performances dans le temps
  - Pourcentages de tir (FG%, 3P%, FT%)
  - Efficacité offensive et défensive
  - Corrélations entre statistiques

---

## Utilisation des Filtres

### Filtres disponibles

Le dashboard dispose de plusieurs filtres interactifs :

#### 1. Filtre par Équipe
- **Emplacement** : Panneau latéral droit
- **Utilisation** : Cliquez sur le nom d'une équipe pour filtrer les joueurs
- **Multi-sélection** : Maintenez Ctrl (Windows) ou Cmd (Mac) pour sélectionner plusieurs équipes

#### 2. Filtre par Position
- **Options** : PG (Meneur), SG (Arrière), SF (Ailier), PF (Ailier fort), C (Pivot)
- **Utilisation** : Cliquez sur une ou plusieurs positions
- **Réinitialisation** : Cliquez sur l'icône de gomme pour effacer le filtre

#### 3. Filtre par Saison
- **Utilisation** : Sélectionnez la saison souhaitée dans le menu déroulant
- **Par défaut** : Affiche la saison la plus récente

#### 4. Filtre par Âge
- **Type** : Curseur (slider)
- **Utilisation** : Ajustez les poignées pour définir une plage d'âge
- **Exemple** : 25-35 ans pour les joueurs en pleine maturité

### Interactions entre visualisations

Les graphiques sont **inter-connectés** :
- Cliquez sur une barre dans un graphique pour filtrer automatiquement les autres visualisations
- Cliquez à nouveau pour désélectionner
- Utilisez Ctrl+clic pour sélectionner plusieurs éléments

---

## Interprétation des Visualisations

### Graphiques principaux

#### 📊 Graphique en barres - Top scoreurs
- **Lecture** : Les joueurs sont classés par ordre décroissant de points par match
- **Couleur** : Code couleur par équipe
- **Interaction** : Cliquez sur une barre pour voir les détails du joueur

#### 🥧 Graphique circulaire - Répartition par position
- **Lecture** : Montre la distribution des joueurs par position
- **Pourcentage** : Affiché pour chaque section
- **Interaction** : Survolez pour voir les détails

#### 📈 Graphique en courbes - Évolution des performances
- **Axe X** : Matchs ou dates
- **Axe Y** : Statistique sélectionnée (points, rebonds, etc.)
- **Légende** : Différents joueurs ou statistiques
- **Zoom** : Faites glisser pour sélectionner une période

#### 🎯 Radar Chart - Profil de joueur
- **Axes** : Différentes compétences (tir, rebonds, passes, etc.)
- **Lecture** : Plus la surface est grande, plus le joueur est polyvalent
- **Comparaison** : Plusieurs joueurs peuvent être superposés

#### 🔥 Heatmap - Corrélations
- **Lecture** : Plus la couleur est intense, plus la corrélation est forte
- **Rouge** : Corrélation positive forte
- **Bleu** : Corrélation négative forte
- **Blanc** : Pas de corrélation

### KPI (Indicateurs clés)

Les cartes KPI en haut du dashboard affichent :
- 📊 **Moyenne de points** : Points moyens par match de tous les joueurs
- 🏀 **Moyenne de rebonds** : Rebonds moyens par match
- 🎯 **Moyenne de passes** : Passes décisives moyennes par match
- ⚡ **Pourcentage de tir moyen** : Efficacité moyenne au tir

---

## Astuces et Conseils

### Pour une meilleure expérience

1. **Mode Plein écran**
   - Appuyez sur F11 ou cliquez sur l'icône plein écran
   - Idéal pour les présentations

2. **Actualisation des données**
   - Pour actualiser : Cliquez sur "Actualiser" dans l'onglet "Accueil"
   - Les données se mettent à jour automatiquement

3. **Export des visualisations**
   - Cliquez sur "..." en haut à droite d'un visuel
   - Sélectionnez "Exporter les données" pour obtenir un CSV

4. **Favoris**
   - Créez des signets pour sauvegarder des vues spécifiques
   - Accès rapide à vos analyses favorites

5. **Mode Focus**
   - Double-cliquez sur une visualisation pour la voir en grand
   - Appuyez sur Échap pour revenir

### Questions fréquentes

**Q : Les données ne s'affichent pas correctement**
- R : Vérifiez que le fichier `stats_par_saison.csv` est bien dans le dossier `data/`

**Q : Comment ajouter de nouveaux joueurs ?**
- R : Ajoutez les données dans le fichier CSV et actualisez le dashboard

**Q : Le dashboard est lent**
- R : Réduisez le nombre de visuels affichés ou filtrez les données

**Q : Comment partager le dashboard ?**
- R : Utilisez Power BI Service pour publier en ligne ou exportez en PDF

---

## Support et Ressources

- **Documentation Power BI** : https://docs.microsoft.com/fr-fr/power-bi/
- **Tutoriels vidéo** : https://www.youtube.com/powerbi
- **Forum communautaire** : https://community.powerbi.com/

---

*Pour toute question ou suggestion, n'hésitez pas à créer une issue sur le dépôt GitHub.*
