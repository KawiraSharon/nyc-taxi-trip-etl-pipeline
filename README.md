# NYC Taxi Trip Data ETL Pipeline

This project implements a full ETL pipeline orchestrated using Kestra. It extracts, transforms, and loads January 2023 NYC Yellow Taxi Trip data from the month of January as sampled from Kaggle, into a dockerized instance of PostgreSQL database managed locally on pgAdmin, and visualizes key insights using PowerBI. Kestra’s script for plugin is used to execute the Extraction, Transformation and Loading tasks.

----------------------------------------------------------------------------------------------------------

## Tech Stack

- **Kestra** – to enable workflow orchestration, the entire script is written in YAML
- **Python** – for extraction from kaggle website using a publicly accessible API key, transformation to a cleaner dataset, and loading onto the psql.
- **PostgreSQL (via Docker)** – the database instantiated on docker as the select database
- **Docker** – instantiate and containerize PostgreSQL
- **Power BI** – enables visualization and storytelling

----------------------------------------------------------------------------------------------------------

## Running the Pipeline

The entire pipeline runs within the [Kestra](https://kestra.io/) orchestration engine. using a Dockerized PostgreSQL environment.

To execute the code locally as a yaml file, please use the command;
```bash
docker-compose up -d
```

Want to see the entire flow of the pipeline? 
[Click here to view the ETL visuals](./documentation/screenshots.md)
