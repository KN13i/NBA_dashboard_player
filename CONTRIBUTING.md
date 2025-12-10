# 🤝 Guide de Contribution

Merci de votre intérêt pour contribuer au projet NBA Player Analytics Dashboard !

## 📋 Table des Matières
1. [Comment Contribuer](#comment-contribuer)
2. [Types de Contributions](#types-de-contributions)
3. [Processus de Contribution](#processus-de-contribution)
4. [Standards de Code](#standards-de-code)
5. [Données et Sources](#données-et-sources)

---

## Comment Contribuer

Nous accueillons toutes les contributions, grandes ou petites :
- 🐛 Signaler des bugs ou problèmes
- 💡 Proposer de nouvelles fonctionnalités
- 📝 Améliorer la documentation
- 🔧 Corriger des bugs
- ✨ Ajouter de nouvelles visualisations
- 📊 Enrichir les données

---

## Types de Contributions

### 1. Signaler un Problème

Si vous trouvez un bug ou avez une suggestion :

1. Vérifiez que le problème n'existe pas déjà dans les [Issues](https://github.com/KN13i/NBA_dashboard_player/issues)
2. Créez une nouvelle issue avec :
   - 📝 Description claire du problème
   - 🔄 Étapes pour reproduire
   - 📷 Captures d'écran si applicable
   - 💻 Version de Power BI utilisée

**Template d'issue** :
```markdown
**Description du problème**
[Description claire et concise]

**Étapes pour reproduire**
1. Ouvrir le dashboard
2. Cliquer sur ...
3. Observer le problème

**Comportement attendu**
[Ce qui devrait se passer]

**Captures d'écran**
[Si applicable]

**Environnement**
- Power BI Desktop version : [ex. 2.123.742.0]
- OS : [ex. Windows 11]
```

### 2. Proposer une Fonctionnalité

Pour proposer une nouvelle fonctionnalité :

1. Ouvrez une issue avec le tag `enhancement`
2. Décrivez :
   - 🎯 L'objectif de la fonctionnalité
   - 💼 Les cas d'usage
   - 📊 L'impact attendu
   - 🔧 Les détails techniques si possibles

### 3. Améliorer la Documentation

La documentation peut toujours être améliorée :
- Corriger des fautes de frappe
- Clarifier des instructions
- Ajouter des exemples
- Traduire en d'autres langues
- Ajouter des screenshots

### 4. Contribuer au Code/Dashboard

Pour modifier le dashboard Power BI :
1. Suivez le [Processus de Contribution](#processus-de-contribution)
2. Testez vos modifications
3. Documentez les changements

---

## Processus de Contribution

### Étape 1 : Fork et Clone

```bash
# Fork le repository sur GitHub

# Cloner votre fork
git clone https://github.com/VOTRE_USERNAME/NBA_dashboard_player.git
cd NBA_dashboard_player

# Ajouter le repository original comme remote
git remote add upstream https://github.com/KN13i/NBA_dashboard_player.git
```

### Étape 2 : Créer une Branche

```bash
# Créer une nouvelle branche pour votre contribution
git checkout -b feature/ma-nouvelle-fonctionnalite

# Ou pour un bug fix
git checkout -b fix/correction-bug-xyz
```

**Convention de nommage des branches** :
- `feature/description` : Nouvelles fonctionnalités
- `fix/description` : Corrections de bugs
- `docs/description` : Modifications de documentation
- `data/description` : Mises à jour de données

### Étape 3 : Effectuer les Modifications

- Modifiez les fichiers nécessaires
- Suivez les [Standards de Code](#standards-de-code)
- Testez vos modifications

### Étape 4 : Commit

```bash
# Ajouter les fichiers modifiés
git add .

# Créer un commit avec un message descriptif
git commit -m "feat: Ajout de la page analyse défensive"
```

**Convention de messages de commit** :
- `feat:` Nouvelle fonctionnalité
- `fix:` Correction de bug
- `docs:` Documentation
- `data:` Mise à jour des données
- `style:` Changements de style/formatage
- `refactor:` Refactoring de code
- `test:` Ajout de tests

### Étape 5 : Push et Pull Request

```bash
# Pousser la branche vers votre fork
git push origin feature/ma-nouvelle-fonctionnalite
```

Ensuite sur GitHub :
1. Aller sur votre fork
2. Cliquer sur "Compare & pull request"
3. Remplir le template de PR :
   - Description des changements
   - Type de changement
   - Tests effectués
   - Captures d'écran si applicable

**Template de Pull Request** :
```markdown
## Description
[Description claire des changements]

## Type de changement
- [ ] Bug fix
- [ ] Nouvelle fonctionnalité
- [ ] Documentation
- [ ] Mise à jour de données

## Tests effectués
- [ ] Testé en local
- [ ] Dashboard s'ouvre correctement
- [ ] Toutes les visualisations fonctionnent
- [ ] Pas d'erreurs dans les données

## Captures d'écran
[Si applicable]

## Checklist
- [ ] Mon code suit les standards du projet
- [ ] J'ai mis à jour la documentation
- [ ] Mes changements ne cassent pas de fonctionnalités existantes
```

---

## Standards de Code

### Dashboard Power BI

#### Structure
- Utiliser des noms de mesures clairs et descriptifs
- Grouper les mesures par catégorie
- Commenter les DAX complexes

#### Nommage
```
✅ Bon : Total_Points_Par_Match
❌ Mauvais : TPPM, calc1, mesure_x
```

#### DAX
- Utiliser des variables pour la lisibilité
- Éviter les calculs imbriqués trop complexes
- Préférer les mesures aux colonnes calculées quand possible

**Exemple de bonne pratique** :
```dax
Moyenne_Points_Par_Match = 
VAR TotalPoints = SUM(Stats[Points])
VAR NombreMatchs = COUNT(Stats[Matchs])
RETURN 
    DIVIDE(TotalPoints, NombreMatchs, 0)
```

### Documentation

#### Markdown
- Utiliser des titres hiérarchiques (# ## ###)
- Ajouter des emojis pour la lisibilité 🎯
- Inclure des exemples de code
- Ajouter des liens vers les ressources

#### Structure des Documents
```markdown
# Titre Principal

## Section 1
Description...

### Sous-section
Détails...

## Section 2
...
```

### Données CSV

#### Format
- Séparateur : virgule (,)
- Encodage : UTF-8
- Première ligne : en-têtes de colonnes
- Pas d'espaces dans les noms de colonnes (utiliser _)

#### Qualité des Données
- Pas de valeurs manquantes (utiliser 0 ou NA si nécessaire)
- Format cohérent (dates, nombres)
- Validation des données avant commit

---

## Données et Sources

### Ajout de Nouvelles Données

Si vous ajoutez des données :

1. **Vérifier la source** : Utiliser uniquement des sources fiables
   - NBA Official Stats
   - Basketball Reference
   - Statistiques vérifiées

2. **Format cohérent** : Respecter le format existant
   - Mêmes colonnes que `stats_par_saison.csv`
   - Même structure

3. **Documentation** : Mettre à jour `data/README.md`
   - Source des données
   - Date de collecte
   - Méthode d'extraction

### Sources Autorisées

✅ **Sources acceptées** :
- NBA.com/stats
- Basketball-reference.com
- API NBA officielle
- ESPN Stats

❌ **Sources non acceptées** :
- Données non vérifiées
- Sources non officielles
- Données scrappées sans autorisation

---

## Processus de Review

Votre Pull Request sera reviewée selon ces critères :

### Checklist de Review
- [ ] Code/Dashboard fonctionne correctement
- [ ] Pas d'erreurs introduites
- [ ] Documentation à jour
- [ ] Style cohérent avec le projet
- [ ] Tests effectués
- [ ] Pas de données sensibles commitées

### Délai de Review
- Les PR sont généralement reviewées sous 3-7 jours
- Les corrections urgentes peuvent être prioritaires
- N'hésitez pas à relancer après 1 semaine

---

## Questions et Support

### Besoin d'Aide ?

- 💬 [Discussions GitHub](https://github.com/KN13i/NBA_dashboard_player/discussions) : Questions générales
- 🐛 [Issues](https://github.com/KN13i/NBA_dashboard_player/issues) : Bugs et problèmes
- 📧 Contact direct : Voir le profil GitHub

### Ressources Utiles

- [Documentation Power BI](https://docs.microsoft.com/fr-fr/power-bi/)
- [Guide DAX](https://dax.guide/)
- [Git Basics](https://git-scm.com/doc)
- [Markdown Guide](https://www.markdownguide.org/)

---

## Code de Conduite

En contribuant, vous acceptez de :
- ✅ Être respectueux envers les autres contributeurs
- ✅ Accepter les critiques constructives
- ✅ Donner du feedback constructif
- ✅ Se concentrer sur ce qui est le mieux pour le projet

---

## Reconnaissance

Tous les contributeurs seront reconnus dans le projet :
- Mention dans les release notes
- Ajout dans la liste des contributeurs
- Remerciements dans le README

---

## Licence

En contribuant, vous acceptez que vos contributions soient sous la même licence que le projet.

---

**Merci de contribuer au projet NBA Player Analytics Dashboard ! 🏀📊**

Chaque contribution, petite ou grande, est précieuse et appréciée ! 🙏
