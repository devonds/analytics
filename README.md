# analytics

This repo contains the code that runs our data model in dbt (data build tool).  It is a collection of SQL and YAML files that dbt uses to update our data model in snowflake.  

# getting started 

You can run dbt either locally or on dbt cloud. That will be connected to our snowflake warehouse via your own credentials, and will allow you to run dbt in a development environment. Development environment create tables within a schema unique to the developer (e.g., dbt_dsampson). When you have tested changes within your development environment, you can submit a pull request. In production, dbt gets code from the main branch and uses it to run queries on snowflake. In production, tables get written to the schema dbt_prod.  

1. dbt Cloud. The easiest way to get started is to develop in dbt's cloud IDE that is already connected to snowflake. The IDE integrates with GitHub to make submitting PRs easy too. Reach out to Devon, Kathryn or Joe to set up a dev account on dbt Cloud. 
2. dbt core. You can also work on the dbt project locally from the IDE of your choice, taking advantage of all that VS Code or Pycharm or whatever has to offer.  Directions for installing the dbt-core python app and connecting it to Snoflake are here. 

# style and project structure 

We follow dbt's best practices[https://docs.getdbt.com/guides/best-practices/how-we-structure/1-guide-overview] for structuring the project.  Please review these before getting started. 

# submitting pull requests 
