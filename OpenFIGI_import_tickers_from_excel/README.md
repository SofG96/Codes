# OpenFIGI API

This script is written in Python, and it shows **how to use the [Open FIGI API](https://www.openfigi.com/api)** to retrieve identifiers of securities issued by governments, financial and non-financial companies.

The script **automatically creates queries importing tickers** (called `BASE_TICKER` in the OpenFIGI API) **from an Excel file**.

The API returns results as nested JSON files. The script also shows **how to flatten out nested JSON files in a easily readable table** that can be readily exported. 


## Getting Started

[Open FIGI](https://www.openfigi.com/) creates **FIGIs**, which stands for Financial Instrument Global Identifier. A FIGI is a globally recognized, non-changing identifier that uniquely identifies a security.

Please read the [API instructions](https://www.openfigi.com/api) to understand how queries shall be made.

Instead, the `map_table` function normalizes nested JSON files. It is easily generalizable to fit also JSON files with more nodes and higher levels of nesting.


### Prerequisites

I recommend to first open the script in Google CoLab, as it does not require any software installation.

If you wish to modify the script to fit your purposes, you will need to download Anaconda Navigator. 


### Installing

The script requires some packages to be installed in your environment. Please write in the Anaconda Prompt:

``` python
conda activate name_env
pip install ast
pip install json         
pip install requests  
```


## Deployment

The final lines of code export the results into an Excel file when using CoLab. Please change those lines, so that the script fits the Python interface you are using. 


## Built With

* [Google CoLab](https://colab.research.google.com/notebooks/intro.ipynb#recent=true) 
* [Open FIGI](https://www.openfigi.com/)


## Authors

* [Sofia Gori](https://github.com/SofiaGori)


