# Dashboard Power BI - NBA Player Analytics

## Fichier Dashboard

**Nom du fichier** : `NBA_Player_Dashboard.pbix`

Ce dossier contient le fichier Power BI Dashboard interactif pour l'analyse des statistiques des joueurs NBA.

## Prérequis

Pour ouvrir et modifier le dashboard :
- **Power BI Desktop** : Téléchargez gratuitement depuis [Microsoft Power BI](https://powerbi.microsoft.com/fr-fr/desktop/)
- **Système d'exploitation** : Windows 10/11 ou supérieur
- **Espace disque** : Au moins 2 GB d'espace libre

## Structure du Dashboard

Le dashboard Power BI inclut :

1. **Page Vue d'ensemble**
   - Statistiques générales des joueurs
   - Classement des meilleurs scoreurs
   - Visualisation des performances par équipe

2. **Page Analyse détaillée**
   - Comparaison de joueurs
   - Évolution des statistiques
   - Filtres interactifs par position, équipe, âge

3. **Page Performances**
   - Pourcentages de tir
   - Efficacité offensive et défensive
   - Graphiques de corrélation

## Sources de données

Le dashboard utilise les données du dossier `data/` :
- `stats_par_saison.csv` : Statistiques principales
- Logos des équipes via API NBA

## Mise à jour des données

Pour mettre à jour les données dans le dashboard :
1. Ouvrir le fichier `.pbix` dans Power BI Desktop
2. Aller dans "Accueil" > "Transformer les données"
3. Actualiser les sources de données
4. Cliquer sur "Fermer et appliquer"

## Publication

Pour partager le dashboard :
- **Power BI Service** : Publier sur le cloud Power BI
- **Export PDF** : Fichier > Exporter > PDF
- **Export PowerPoint** : Fichier > Exporter > PowerPoint

## Note

Le fichier `.pbix` n'est pas inclus dans ce dépôt Git en raison de sa taille.
Il peut être téléchargé séparément ou recréé en suivant la documentation dans le dossier `docs/`.
