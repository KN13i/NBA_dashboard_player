# NBA_dashboard_player
Dashboard interactif sur power BI sur l'analyse statistique des joueurs NBA

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![NBA](https://img.shields.io/badge/NBA-253B73?style=for-the-badge&logo=nba&logoColor=white)
---

Ce projet présente un **dashboard interactif Power BI** représentant l'ensemble des joueurs NBA sur la saison 2024-2025.
Dans ce dashboard, on a rendu sur :
  - L'évolution des joueur depuis la saison 2020 sur ses statistiques dont son nombre de matchs, 
sa réussite au tir ou encore son nombre de points marqués en moyennes par saisons.

  - Caractéristiques d'un joueur


## Objectif de ce Dashboard
Ce projet présente un **dashboard interactif Power BI** représentant l'ensemble des joueurs NBA sur la saison 2024-2025.
Dans ce dashboard, on a rendu sur :

### Comparaison les statistiques d'un joueur
- Comparaison statistiques sur l'effacicité au tir, le nombre de points par rapport aux joueurs sur le même poste
- Affichage des caractéristiques des joueurs
- Notation des joueurs sur les aspects clés en NBA (shooting, defense, playmaking...)

### Analyse des performances 
- Identifier les forces et faiblesses des joueurs (radar chart)
- Visualisation de l'évolution des performances sur les 5 dernières saisons

### Compétences sur Power BI
- Création de graphiques interactives 
- Jointure de tables SQL
- Apprentissage du langague DAX et Power Query

---

##  Structure du Projet

```
NBA_dashboard_player/
│
├── README.md                          
│
├── data/                             
│   ├── stats_par_saison.csv          
│   ├── head_players.png                   
│
├── dashboard/                        
│   ├── NBA_Player_Dashboard.pbix     
│   ├── README.md
│   ├── Screenshoots                
│
        
```

---

##  Aperçu du Dashboard

<img width="1307" height="735" alt="image" src="https://github.com/user-attachments/assets/ca363c97-da2b-4b0d-ae01-a4cb96b3fe1c" />

---
##  Améliorations Futures
- Automatiser la collecte de données avec Python et GCP
- Actualisation hebdomadaire des stats sur la saison 2025-2026
  
---

## Sources de Données
- Basketball Reference = stats par saisons
- RapidApi = logos des équipes
- GreenGuitarO = têtes des joueurs NBA
