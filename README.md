# constituents_ETL

This app is designed to aggregate data from three csv files in its working directory and then produce two csv files containing the aggregated data, also in the working directory.

## "Pre-Flight" checklist:

- Install the Anaconda distribution of Python
  - **https://www.anaconda.com/products/individual**
  - This app was built using Python 3.8.8 and Conda 4.10.3
- Install Pandas
  - run **conda install pandas** in your terminal
  - This app was built using Pandas 1.2.5
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
    - "is_primary": *boolean* (1 or 0)
    - "email": *string*
    - "status": *boolean* (1 or 0)
  - ***cons_email_chapter_subscription.csv***, has to include the following columns:
    - "cons_email_chapter_subscription_id": *int*
    - "cons_email_id": *int*
    - "chapter_id": *int*
    - "isunsub": *boolean* (1 or 0)

## Instructions:

- Download the zipped project.
- Extract the file *cons_pipeline.ipynb* into your working directory (the directory containing your raw data files).
- In your terminal, run the command **jupyter notebook**. This will open your local directory in jupyter notebooks on your browser.
- Within jupyter notebooks, navigate to your working directory and open *cons_pipeline.ipynb*
- Follow the instructions in the notebook to run the pipeline.
