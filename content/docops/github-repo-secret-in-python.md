---
title: "Use Github Repo Secret in Python (without Action)"
description: ""
date: 2023-06-30T18:17:35Z
tags: ["Python"]
---

## The problem to solve

Every month there is a task to update exchange rates in a markdown file. All there is to do is to send an API request to get the foreign exchange rates and currency conversion, extract the data from the response, and then format it.

A perfect job for Python! The only challenge is that we do not want to include API key in the Python script. How to handle that?

## Access environment variables using the os module

If you google "how to use github secrets and variables in python", almost all the answers talk about GitHub Actions/workflows. But, does it have to be so? ChatGPT just showed me, "No!"

> When you add the XXX API access key as a repository secret in GitHub, you can access it within your Python script by using the os module to access environment variables. Here's how you can refer to the access key in your script:

```python
import os

access_key = os.environ.get('YOUR_PET_API_ACCESS_KEY')

# Check if the access key is available
if access_key is None:
    print("PET API access key not found. Please set the 'YOUR_PET_API_ACCESS_KEY' environment variable.")
    exit()
```

## The full script

Here is the full script that returns the exchange rates on the last day of the previous month. (Courtesy to ChatGPT!)

```python

import requests
import os
from datetime import date, timedelta

access_key = os.environ.get('FIXER_API_KEY')
symbols = "EUR,GBP,CAD,AUD"


# Check if the access key is available
if access_key is None:
    print("Fixer API key not found. Please set the 'FIXER_API_KEY' environment variable.")
    exit()

# Get the last day of the previous month
today = date.today()
first_day_of_month = date(today.year, today.month, 1)
last_day_of_previous_month = first_day_of_month - timedelta(days=1)

# Format the date in YYYY-MM-DD format
date_string = last_day_of_previous_month.strftime("%Y-%m-%d")

# Make a Fixer API request
base_url = f"http://data.fixer.io/api/{date_string}?access_key={access_key}&base=USD&symbols={symbols}"
response = requests.get(base_url)

# Check if the request was successful
if response.status_code == 200:
    # Store the rates object in a string
    rates = response.json()["rates"]

    # Remove the currency code and join the rates using a pipe
    rates_string = " | ".join([str(rate) for rate in rates.values()])

    # Format the month
    previous_month = "**" + last_day_of_previous_month.strftime("%B") + "**"

    print("Exchange rates on", date_string, ": |", previous_month, "|", rates_string, "|")
else:
    print("Failed to retrieve exchange rates. Error:", response.status_code)

```