# OCR - Projet 4 
## Audit d’un environnement de données

Projet réalisé dans le cadre de la formation **Data Engineer** d’OpenClassRoom.  
Aout - Septembre 2025 

---

## Contexte du projet (situation fictive)

Une chaîne de supermarchés personnalise l’expérience en magasin grâce au suivi des comportements clients (coupons promotionnels personnalisés, recommandations basées sur les historiques d’achat, etc.).
Une équipe de data analysts suit les ventes (types de produits, prix, employés, clients, etc.).
Des incohérences dans les chiffres d'affaires remontés ont été observées par le pôle BI.

En tant que **data engineer** , il est demandé de comprendre et d'analyser les flux de données de l’entreprise.
L'objectif du projet est d’identifier les problèmes actuels et de réaliser une Proof of Concept (POC) intégrant des recommandations garantissant la sécurité et la qualité des données de l'entreprise.


## Travail réalisé

1. **Analyse de l'architecture de données de l'entreprise** :
    - Database en temps réel - SQLserver
    - Agrégation des données dans un Cube OLAP - Azure Analysis Services
    - Visualisation des résultats - PowerBI
      
2. **Création d'un dictionnaire et d'un schéma des données du cube OLAP**
   
3. **Réalisation un prototype en local avec les données du cube OLAP**
    - Chargement des données dans PostGreSQL
    - Requêtes métiers pour vérifier le chiffre d'affaire
   
4. **Compréhension des problèmes sur la base des logs**
   - Analyse de la table de logs
   - Itération des hypothèses
   - Identification du problème de non atomicité des données  
  
8. **Proposition de recommandations et d'un plan d'action**
   - Proposition de 6 recommandations pour sécurisé le flux de données
      - A déployer au court terme : amélioration de la table de log, atomicité des transaction, contraintes d'intégrité, gestion des droits...
      - A déployer au moyen terme : Monitoring ETL - Trigger
    - Intégration de ces recommandations dans le POC

9. **Rédaction d'un rapport d'Audit**  


---

## Outils 
-`Python`
-`PostgreSQL`  
-`SQL architect`

