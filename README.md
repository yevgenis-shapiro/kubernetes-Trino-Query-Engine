<img width="1500" height="1125" alt="dbt-trino-architecture" src="https://github.com/user-attachments/assets/3a04392d-dabf-4e19-b5a2-aef85b40c5a7" />



## Kubernetes | Trino SQL Query Engine
Trino (formerly known as PrestoSQL) is an open-source, distributed SQL query engine designed for running fast, interactive analytics on large datasets across multiple data sources.


#### 🧩 Key Features: :
   - **Query federation**: Combine data from multiple sources (e.g., join S3 and PostgreSQL tables).
   - **High performance**: In-memory distributed query execution.
   - **ANSI SQL compatible**: React UI for search, lineage visualization, and dataset exploration.
   - **Scales horizontally**: Add more worker nodes to handle larger queries.
   - **Connectors**: AWS S3, GCS, HDFS , Hive, Iceberg, Delta Lake , MySQL, PostgreSQL, MongoDB , Kafka, Elasticsearch


🧠 Architecture Overview:

✅ Coordinator Node – Parses queries, plans execution, and schedules work.
✅ Worker Nodes – Execute query tasks and process data.
✅ Catalogs & Connectors – Define how Trino connects to external systems.

     

🚀 Deployment Options
```
terraform init
terraform validate
terraform plan -var-file="template.tfvars"
terraform apply -var-file="template.tfvars" -auto-approve
```




