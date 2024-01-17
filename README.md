# Twitter-Data-ETL-Pipeline-using-Apache-Airflow

## Introduction

This project focuses on creating an ETL pipeline that extracts tweets from specified user timelines using the Tweepy library, transforms the data into a structured format, and loads it for further analysis. Leveraging the robustness of Python and the scheduling capabilities of Apache Airflow, we've created a scalable solution to handle Twitter data efficiently.

## Technology Stack

- **Python**: The backbone of our ETL process, utilized for scripting and data manipulation.
- **Tweepy**: A Python library for accessing the Twitter API.
- **Apache Airflow**: Used for orchestrating the ETL pipeline with scheduled workflows.
- **Pandas**: For data transformation and CSV file generation.

## Usage

1. **twitter_etl.py**: Defines the function `run_twitter_etl()` which authenticates with the Twitter API and fetches the tweets.
2. **twitter_commands.sh**: Contains the necessary commands to set up the environment for running the ETL pipeline.
3. **twitter_dag.py**: Defines the DAG for Airflow and sets up the scheduling for the ETL task.

To execute the ETL process manually, run:

```python
python twitter_etl.py
```

For scheduling the process, place the `twitter_dag.py` in your Airflow dags folder and ensure Airflow is running.

## Data

This ETL pipeline is designed to fetch tweets from a specific Twitter user, as defined in `twitter_etl.py`. The output is a CSV file that includes tweet text, favorite count, retweet count, and creation time.


## Acknowledgments

Special thanks to all the contributors and maintainers of the open-source libraries used in this project. 
