



# Yeshurun Second Degree final project 
Creating a backtest for comparing augmented linear regression vs buy and hold 

## More info 
This project will create backtest for comparing 2 investing strategies 
the first is 'Buy N Hold '
the second is prediction via regression 

## This project is an extension of cash_analysis 

here is the link for the parent project 
[CashAnalysis](https://barakdiker123.github.io/CashAnalysis/)

# How to install N Upload packages 
For exporting the environment one should 

``` sh
conda env export -n yesh_thesis > env.yml
```

Create a new environment from the env.yml file 
``` sh
conda env create -n yesh_thesis --file env.yml
```


How to upload the new distribution 


``` sh

conda activate yesh_thesis 

python3 -m twine upload --repository testpypi dist/*

python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps stock_prediction_barakdiker
```

and in order to run the test function do 

``` python
from stock_prediction_barakdiker import regression_calculator
regression_calculator.add_one(1)

```







## Credits 

* Barak Nadav Diker 
* Yeshurun 
