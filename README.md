# Dataform Project - Dataform-git

## Overview
This project transforms raw event tracking data into clean and report ready tables in BigQuery using google provided public dataset.

## Project Setup
- The project uses BigQuery as the data warehouse.
- The raw data is sourced from google provided public dataset and processed through various stages as Bronze,silver and gold where we have created
  a view to reference raw data and created a clean table with all the transformations and a report table with aggregate data as per the requirement.

## Structure
- Raw Data: Contains the raw events data (`vw_stg_raw_events.sqlx`).
- Clean Data: Contains the clean data (`purchase_traffic_source_medium.sqlx`).
- Report Data: Contains the aggregate data (`top_traffic_source_medium.sqlx`).

## Dependencies
- BigQuery for the data warehouse.
- Dataform for the data transformation pipeline.
- Github for version and collabration in dataform.
- IAM for giving permissions to service account to execute dataform code and github setup.
- Secret Manager to generate a secret token to configure github.