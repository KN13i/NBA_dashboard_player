# Sources de Données

## Fichiers de données

### stats_par_saison.csv
Ce fichier contient les statistiques par saison des joueurs NBA, incluant :
- **Joueur** : Nom du joueur
- **Saison** : Année de la saison
- **Equipe** : Équipe actuelle du joueur
- **Position** : Position sur le terrain (PG, SG, SF, PF, C)
- **Matchs_Joues** : Nombre de matchs joués
- **Minutes_Par_Match** : Moyenne de minutes par match
- **Points_Par_Match** : Moyenne de points par match
- **Rebonds_Par_Match** : Moyenne de rebonds par match
- **Passes_Par_Match** : Moyenne de passes décisives par match
- **Interceptions_Par_Match** : Moyenne d'interceptions par match
- **Contres_Par_Match** : Moyenne de contres par match
- **Pourcentage_Tir** : Pourcentage de réussite au tir (%)
- **Pourcentage_3Points** : Pourcentage de réussite à 3 points (%)
- **Pourcentage_LF** : Pourcentage de réussite aux lancers francs (%)
- **Age** : Âge du joueur

**Source** : Données basées sur les statistiques officielles de la NBA 2023-24

### head_players.png
Image des meilleurs joueurs NBA utilisée pour l'en-tête du dashboard.

## Logos des équipes

Les logos des équipes NBA sont obtenus via l'API officielle NBA :
- **API NBA** : `https://stats.nba.com/`
- **Endpoint logos** : `https://cdn.nba.com/logos/nba/{team_id}/primary/L/logo.svg`

### Liste des équipes NBA principales :
- Los Angeles Lakers (team_id: 1610612747)
- Golden State Warriors (team_id: 1610612744)
- Boston Celtics (team_id: 1610612738)
- Phoenix Suns (team_id: 1610612756)
- Milwaukee Bucks (team_id: 1610612749)
- Denver Nuggets (team_id: 1610612743)
- Philadelphia 76ers (team_id: 1610612755)
- Dallas Mavericks (team_id: 1610612742)
- Miami Heat (team_id: 1610612748)
- Los Angeles Clippers (team_id: 1610612746)
- Cleveland Cavaliers (team_id: 1610612739)
- Oklahoma City Thunder (team_id: 1610612760)
- Minnesota Timberwolves (team_id: 1610612750)
- Atlanta Hawks (team_id: 1610612737)
- Chicago Bulls (team_id: 1610612741)
- Indiana Pacers (team_id: 1610612754)

## Mise à jour des données

Les données peuvent être mises à jour en utilisant :
1. **API NBA Stats** : https://stats.nba.com/stats/
2. **Basketball Reference** : https://www.basketball-reference.com/
3. **NBA Official Stats** : https://www.nba.com/stats/

## Format des données

Toutes les données sont au format CSV avec séparateur virgule (,) et encodage UTF-8.
