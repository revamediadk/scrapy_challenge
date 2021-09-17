# scrapy_challenge

This project is part of the job interview for joining Rentola's spiders team. You will need to use this project as the basic structure/template to implement a spider to crawl `https://londonrelocation.com/properties-to-rent/`.

We are heavily using Python and Scrapy framework in Rentola and thus we are providing the basic structure for your to utilize the same tools to scrap the website.

Your goal is to be able to:
1. Traverse the areas with their links listed in this page `https://londonrelocation.com/properties-to-rent/` such as `Fulham`, `Canary Wharf` `Angel`, and etc. (Already Implemented by us as an example)
2. Visit each area link and traverse the paginated properties lists (page 1 and page 2 only are sufficient).
3. Do not hard code the pages links in step2, scrap them from the area page from step1.
4. For each property you need to save the property title and price per month.

The output should be a JSON file with a list of all properties scraped.

## Setup Instructions (Ubuntu)

Clone this project into your own Github project and submit the project as a part of your job application.

NOTE: Do not fork the project directly as Github will connect your repo to this repo and will help other candidates to easily cheat and learn from your code.

```bash
apt install python3-virtualenv libpython3.8-dev
apt-get install build-essential
```

Create a virtual env and setup dependencies/requirements:
```bash
virtualenv venv -p python3
source venv/bin/activate
pip install -r requirements.txt
```

## Run Scrapy

```bash
# Please submit the londonrelocation.json content to us in the application form
scrapy runspider londonrelocation.py -o londonrelocation.json
```
