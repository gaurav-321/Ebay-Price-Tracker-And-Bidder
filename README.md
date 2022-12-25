# eBay price tracker
This is a Python script that tracks prices for specific items on eBay and sends notifications via xdroid.net API when the price falls within a specified range.

## Requirements
- Python 3
- ebaysdk library
- xdroid.net API key
- eBay API ID
##  Usage
- Edit the API_ID and API_KEY_NOTIFY variables at the top of the script with your eBay API ID and xdroid.net API key, respectively.
- Modify the search_list variable to contain a list of tuples with the following format: (query, min_price, max_price). This will specify the search query and the price range to track for each item.
- Run the script. It will continuously scrape eBay for the specified items and send notifications when the price falls within the specified range.
## Note
This script is set up to search on the German eBay site (ebay.de). If you want to search a different site, modify the api = Connection() line to include the desired domain (e.g. api = Connection(domain="svcs.ebay.com") for the US site).
