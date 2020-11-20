# Rainbow Pages Sri Lankan Business Details Scraper

Rainbowpages.lk Web Scraper written in Python and LXML to extract business details available based on a particular category and location.


## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Fields to Extract

This rainbowpages scraper can extract the fields below:

1. Business Name
2. Phone Number
3. Business Page
4. Address

### Prerequisites

Package requirements:

 - lxml
 - requests

### Installation

Install Python if you dont have it already: https://www.python.org/downloads/

1. Install PIP from: (https://pip.pypa.io/en/stable/installing/) 

2. Install Python Requests, to make requests and download the HTML content of the pages. In cmd, run: 
````
pip install requests
````
 or install from (https://requests.readthedocs.io/en/master/user/install/#install)

3. Install Python LXML, for parsing the HTML Tree Structure using Xpaths. In cmd, run:
```
pip install lxml 
```
or install from (http://lxml.de/installation.html)

## Running the scraper
We would execute the code with the script name followed by the positional arguments **keyword** and **place**. Here is an example
to find the business details for restaurants in Colombo

Open cmd and run:

```
python rainbow_pages.py Restaurants Colombo
```
- Keyword: Restaurants 
- Location: Colombo


This script scrapes according to the keyword provided as a parameter. Thus, it may include situations like below:
Keyword: "PUB" and
Location: "Colombo"
Results may have "pubudu engineering Colombo".

### Solution: Work with Categories available in Rainbowpages site
Rainbow Pages has multiple categories and subcategoris (available here: https://rainbowpages.lk/).

If you know the exact category name you need to scrape, run the script in the following format:

```
python rainbow_pages_category.py Restaurants Colombo
```
- Categroy Name: "Restaurants"
- Location: "Colombo"


## Output

The scripts will create a csv file with the 1. Business Name 2. Phone Number 3. Business Page and 4. Address


 
 
