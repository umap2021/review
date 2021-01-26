This repository contains source code to reproduce our work, submitted for review.

# Installation

This Project requires that you have Python 3.8.1 installed. If you do not have it installed, you can download it [here](https://www.python.org/downloads/release/python-381/).

## To Setup a Python 3  Virtual  Environment
After you have installed Python, you can run the following in your Terminal

```python3 -m venv /path/to/new/virtual/environment```

Example:

```python3 -m venv venv```

## Activate Virtual Environment
Run the following in your Command prompt /Terminal
### For Windows
```bash
source /path/to/new/virtual/environment/Scripts/activate
```
Example:
```bash
venv/Scripts/activate
```

### For Linux and MacOS
```bash
source /path/to/new/virtual/environment/Scripts/activate
```
Example:

```bash
source venv/Scripts/activate
```

### Install necessary Libraries

```bash
python -m pip install -r requirements.txt
```

### Running Script_All_Algo.py

For Amazon Games:
SVD:
```python Script_All_Algo.py --algorithm='SVD' --data_path=AMZGamesDF.csv --df_='AMZG_' --n_tmonths=18 --n_train=10 --user_column='userId' --item_column='productId' --max_rank=80```

PSI:
```python Script_All_Algo.py --algorithm='PSI' --data_path=AMZGamesDF.csv --df_='AMZG_' --n_tmonths=18 --n_train=10 --user_column='userId' --item_column='productId' --max_rank=80```

For Amazon Beauty:
SVD:
```python Script_All_Algo.py --algorithm='SVD' --data_path=AMZBeautyDF.csv --df_='AMZB_' --n_tmonths=18 --n_train=10 --user_column='userId' --item_column='productId' --max_rank=80```

PSI:
```python Script_All_Algo.py --algorithm='PSI' --data_path=AMZBeautyDF.csv --df_='AMZB_' --n_tmonths=18 --n_train=10 --user_column='userId' --item_column='productId' --max_rank=80```


For MovieLen:
```unzip MovieLenDF.zip```

SVD:
```python Script_All_Algo.py --algorithm='SVD' --data_path=MovieLenDF.csv --df_='ML_' --n_tmonths=14 --n_train=6 --user_column='userId' --item_column='movieId' --max_rank=80```

PSI:
```python Script_All_Algo.py --algorithm='PSI' --data_path=MovieLenDF.csv --df_='ML_' --n_tmonths=14 --n_train=6 --user_column='userId' --item_column='movieId' --max_rank=80```


