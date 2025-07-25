# Liquibase

Migrations com liquibase

## Instruções


```sh
liquibase init start-h2 
liquibase init project
liquibase --defaultsFile=migrations/liquibase.properties validate
liquibase --defaultsFile=migrations/liquibase.properties status --verbose
liquibase --defaultsFile=migrations/liquibase.properties updateSQL
liquibase --defaultsFile=migrations/liquibase.properties update 

```

* DBMS

- https://docs.liquibase.com/concepts/changelogs/attributes/dbms.html

* SQL Formats

- https://docs.liquibase.com/concepts/changelogs/sql-format.html

* Variables

- https://docs.liquibase.com/concepts/changelogs/property-substitution.html

* Databases

- https://contribute.liquibase.com/extensions-integrations/directory/database-tutorials/

## Grants

```sh
# Concede permissão para criar jobs
gcloud projects add-iam-policy-binding study-gcp-398200 \
  --member="serviceAccount:study-gcp-398200@appspot.gserviceaccount.com" \
  --role="roles/bigquery.jobUser"

# Concede permissão para alterar dados e tabelas
gcloud projects add-iam-policy-binding study-gcp-398200 \
  --member="serviceAccount:study-gcp-398200@appspot.gserviceaccount.com" \
  --role="roles/bigquery.dataEditor"
```

## References

- https://www.liquibase.com/