# Qantas Hotels Rate Extractor
 This script is designed to extract hotel room rates from Qantas Hotels' website by leveraging their internal API.

# Requirements
- Python 3

# How to run
### Locally
1. Run `pip install pandas requests`
2. Run `python qantas_scrape_requests.py`

### With python virtual enviroment
1. Install venv
2. Run `python -m venv env`
3. Activate the environment: `env/Scripts/Activate.ps1` for Windows, `source env/bin/activate` for linux/Mac
4. Run `pip install -r requirements.txt`
5. Run `python qantas_scrape_requests.py`

# How it Works
- Reads the Details.csv file, which contains hotel details.
- Constructs a URL for each hotel entry based on the hotel ID, check-in, and check-out dates.
- Makes a GET request to Qantas Hotels' internal API using the constructed URL.
- Parses the response and extracts the desired hotel rate information storing it into a list of rates.
- Prints the extracted information in a structured JSON format.

