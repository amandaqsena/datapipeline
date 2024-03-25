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

#A Architecture

Airflow has 4 main components that must be running for it to function properly. These are the web server, scheduler, database, and executor.

The **web server** is a server made with Flask, a Python web framework, that serves to present us with Airflow's user interface. Therefore, it is through it that we access this interface.

The **scheduler** is responsible for scheduling the execution of tasks in the DAGs, so it determines which tasks will be carried out, where they will be executed, and in what order this will happen.

The **database**, in turn, serves to store all the metadata related to the DAGs. As such, it records the time tasks were executed, how long each task took to complete, and the status of each one - whether they were executed successfully or failed, among other related information.

Finally, we have the **executor**, which is the mechanism for executing tasks. That is, it is responsible for determining what resources will be needed to execute these tasks.

using python 3.9 in a virtual environment

define constraint file and install airflow

```
pip install 'apache-airflow==2.3.2' --constraint "https://raw.githubusercontent.com/apache/airflow/constraints-2.3.2/constraints-3.9.txt"
```

export environment variable, we will need to export everytime we need to run
```
export AIRFLOW_HOME=~/Documents/datapipeline
```

Then execute

```
airflow standalone
```