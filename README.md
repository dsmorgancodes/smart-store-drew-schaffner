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