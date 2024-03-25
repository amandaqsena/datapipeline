# datapipeline

Airflow Studies

Project that:

- Uses an API with climate data;
- Extracts weather forecast data;
- Creates a folder using Python;
- Saves the extracted files in CSV format.

Airflow

Used to automate processes
- Open-source tool
- Workflow orchestrator
- Creates, schedules, and monitors pipelines
- Dynamic
- Extensible
- Scalable
- Elegant

Common use cases:
- ETL/ELT pipelines
- ML model training
- Automated report generation
- Automated Backups

DAG: workflow. A data pipeline is a DAG.
Task: the most basic unit of a DAG.
Task instance: the execution of a task at a specific point in a DAG.
Operator: building blocks, encapsulate the logic to perform a unit of work.
