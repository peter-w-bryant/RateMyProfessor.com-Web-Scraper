# RateMyProfessor.com-Web-Scraper
A Python script that uses Selenium to scrape all professor ratings from RateMyProfessor.com provided a unique school ID.

## Usage

From Project directory:
`python3 rmp_scrape/fetcher.py -s <SID>`

Flags:
`-s, --sid`             Specify the RMP school id
`-f, --file_path`       Specify the file path to store the scraped data
`-t, --statistics`      Run and Print the statistics of the School
`-config, --congfig`    Specify the config file path if you want to use a config 
                        file instead of specifying the arguments

Either set a unique school id (sid) for RateMyProfessor.com or pass it as an argument when running the script. The script will then scrape all professor ratings from the school and save them to a CSV file.

From the project directory, run `python3 rmp_scrape/fetch.py -s 1256` to scrape all professor ratings from the University of Wisconsin-Madison. The CSV file will be saved to the project directory in the `static_data/<school_name>_professors.csv` file. 

The statistics flag can be placed at the end of the command line argument. 
The calculations made will be for the average rating, difficulty, and % that would take again per department.