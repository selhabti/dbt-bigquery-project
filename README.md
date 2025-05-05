# dbt-bigquery-project
# Pourquoi c’est important ?
dbt et ses plugins doivent être compatibles (même version majeure et mineure).
Si tu utilises BigQuery, il te faut le plugin dbt-bigquery (et non dbt-postgres).

# Comment corriger ?
## 1. Mettre à jour dbt-core et installer le bon plugin
Si tu utilises BigQuery, exécute :

bash
```
pip install --upgrade dbt-bigquery
```
Cela va :

Mettre à jour dbt-core à la dernière version compatible
Installer le plugin dbt-bigquery (et désinstaller les autres si besoin)
## 3. Vérifier la version
Après installation, vérifie :

bash

dbt --version
Tu dois voir dbt-core et dbt-bigquery à la même version (par exemple 1.9.4).
