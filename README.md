## Setup

1. Unzip python zip file

2. Edit [`config.ini`](EtradePythonClient/etrade_python_client/config.ini)
with your consumer key and consumer secret; copy these from your application's keys' section

3. Create the virtual environment by running the Python's venv command; see the command syntax below

```
$ python -m venv .venv
```

4. Activate the Python virtual environment

On Windows, run:

```
$ .venv\Scripts\activate.bat
```

On Unix or Mac OS, run:

```
$ source .venv/bin/activate
```

5. Use pip to install dependencies for the sample application

```
$ pip install -r requirements.txt
```

To save dependencies

pip freeze > requirements.txt

6. Run the sample application

```
$ python test.py
```


# firstrade-api

A reverse-engineered python API to interact with the Firstrade Trading platform.

This is not an official api! This api's functionality may change at any time.

This api provides a means of buying and selling stocks through Firstrade. It uses the Session class from requests to get authorization cookies. The rest is done with reverse engineered requests to Firstrade's API.

In order to use Fractional shares you must accept the agreement on the website before using it in this API.

---

## Contribution

Please feel free to contribute to this project. If you find any bugs, please open an issue.

## Disclaimer
I am not a financial advisor and not affiliated with Firstrade in any way. Use this tool at your own risk. I am not responsible for any losses or damages you may incur by using this project. This tool is provided as-is with no warranty.

## Setup

Install using pypi:

```
pip install firstrade
```

## Quikstart

The code in `test.py` will:
- Login and print account info.
- Get a quote for 'INTC' and print out the information
- Place a dry run market order for 'INTC' on the first account in the `account_numbers` list
- Print out the order confirmation
- Contains a cancel order example
- Get an option Dates, Quotes, and Greeks
- Place a dry run option order
---

## Implemented Features

- [x] Login (With all 2FA methods now supported!) 
- [x] Get Quotes
- [x] Get Account Data
- [x] Place Orders and Receive order confirmation
- [x] Get Currently Held Positions
- [x] Fractional Trading support (thanks to @jiak94)
- [x] Check on placed order status. (thanks to @Cfomodz)
- [x] Cancel placed orders
- [x] Options (Orders, Quotes, Greeks)
- [x] Order History

## TO DO

- [ ] Test options fully
- [ ] Give me some Ideas!

## Options

### I am very new to options trading and have not fully tested this feature.

Please:
- USE THIS FEATURE LIKE IT IS A ALPHA/BETA
- PUT IN A GITHUB ISSUE IF YOU FIND ANY PROBLEMS
  
## If you would like to support me, you can do so here:
[![GitHub Sponsors](https://img.shields.io/github/sponsors/maxxrk?style=social)](https://github.com/sponsors/maxxrk)