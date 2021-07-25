# constituents_ETL

This app is designed to aggregate data from three csv files in its working directory and then produce two csv files containing the aggregated data, also in the working directory.

## "Pre-Flight" checklist:

- Install the Anaconda distribution of Python
  - **https://www.anaconda.com/products/individual**
  - This app was built using Python 3.8.8 and Conda 4.10.3
- Install pandas
  - run **conda install pandas** in your terminal
  - This app was built using Pandas 1.2.5

## Instructions:

- Download the zipped project.
- Extract the file *cons_pipeline.ipynb* into your working directory.
- Ensure your working directory contains the following files:
  - ***cons.csv***, has to include the following columns:
    - "cons_id": *int*
    - "source": *string*
    - "subsource": *string*
    - "is_validated": *boolean* (1 or 0)
    - "is_banned": *boolean* (1 or 0)
    - "create_dt": *datetime*
    - "modified_dt": *datetime*
    - "status": *boolean* (1 or 0)
  - ***cons_email.csv***, has to include the following columns:
    - "cons_email_id": *int*
    - "cons_id": *int*
    - "is_validated": *boolean* (1 or 0)
    - "is_primary": *boolean* (1 or 0)
    - "email": *string*
    - "status": *boolean* (1 or 0)
  - ***cons_email_chapter_subscription.csv***, has to include the following columns:
    - "cons_email_chapter_subscription_id": *int*
    - "cons_email_id": *int*
    - "chapter_id": *int*
    - "is_unsub": *boolean* (1 or 0)



cons_email_chapter_subscription_id	   cons_email_id   	chapter_id	   isunsub	   unsub_dt	   modified_dt
