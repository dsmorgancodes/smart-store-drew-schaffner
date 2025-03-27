# smart-store-drew-schaffner

## Spinning Up Python
First, we must initialize our virtual environment. Without a virtual environment running, python can only be run from our device directory and we would prefer to keep thing running only in our project when possible. 

To create a new environment we can simple run: 

```shell
python3 -m venv .venv
```

```shell
source .venv/bin/activate
```

## Python Set Up
First, we need to make sure that we have configured out dependencies. In this case, this is straightforward since we have been giving a requirements.txt file with everything we will need. 

```shell
python3 -m pip install --upgrade -r requirements.txt
```
The command -r requirements.txt is a great command as it updates our virtual environment withatever dependencies are contained in our requirements.txt file. This is a much much faster way of checking in dependencies when we run our venv. Using our requirement file will enable us to keep our dependencies in order. 

## Test Our System
Using the script from our requirements file: 

```shell
python3 -m datafun_venv_checker.venv_checker
```

We can verify that we have installed all the rquired packages. 

## Run Python Scripts
Now that we have prepared our project, we can run scripts. 

```shell
python3 scripts/data_prep.py
```

This runs any script at the end of the file path if the title is correct. 

## Data Cleaning
Data cleaning is the process by which we clean data and prepare it for ETL. I've made a few comments in my python scripts to help myself with the code flow. Some of the more notable comments are: 

Dr. Case has configured her files so that the file paths of the python scripts form the file paths to where the raw data is found. This is super convenient as it enables our scripts to be used with many different data sets. By adding data to raw an a script to data_preparation we can utilize prewritten code. This is the naming convention: 

For Scripts - The name of .py file much match the name in the Raw Data Folder. 

### Example
If we were to have data for Bike Sales in our raw folder, our Data Preparation script for this file would be titled: 

```shell
prepare_bike_sales_data.py
```

This would be the script for the file located in the raw folder at: data/raw/bike_sales_data.csv

It is worthy to note that if we get the name wrong or if we ruin case sensitivity that this will not function. 

## Creating a Data Scrubbing Script

I modified an existing script that I found in Dr. Case's repository. It ran all these data cleaning operations under one script. I removed the customer data script and the products data script as we already had these. My new script that I have created is useful for forcing dates to be formatted a particular way. 