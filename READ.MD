## Custom ASYNC Scraper - Hyatt Place & Hyatt Regency
Extracting merchant data from Hyatt websites can be challenging due to their security measures. Below is an alternative method to extract data from Hyatt Place and Hyatt Regency.

### Hyatt Regency
Follow these steps to extract data:
1. **Visit the Website:** Go to `https://www.hyatt.com/hyatt-regency/en-US/bhmhr-hyatt-regency-birmingham-the-wynfrey-hotel`.
2. **Access Location Drop Down:** In the website's navigation section, click on the Location drop-down menu. This will display all the USA locations.
3. **Save the Webpage:** Save the HTML webpage manually.
4. **Extract URLs:** Use a Python script (`brands_scraper/scraper_scripts/hyattregency/hyattregency_script.py`) to extract all location URLs from the saved HTML page. The extracted URLs will be saved in `brands_scraper/scraper_scripts/hyattregency/hyattregency_urls.csv`.
5. **Collect Cookies and Headers:** Collect the cookies and headers from `https://www.hyatt.com/hyatt-regency/en-US/bhmhr-hyatt-regency-birmingham-the-wynfrey-hotel`.
6. **Get a Second Set of Cookies and Headers:** To avoid IP blocks after few Requests, collect a second set of cookies and headers. Use the Opera browser with an Americas or any other Region VPN enabled and revisit the URL to get this second set.
7. **Configure Main Script:** Configure both sets of collected cookies and headers in the main script located at `brands_scraper/scraper_scripts/hyattregency/main.py`.

### Hyatt Place
Follow these steps to extract data:
1. **Visit the Website:** Go to `https://www.hyatt.com/en-US/hotel/arizona/hyatt-place-scottsdale-north/phxzs`.
2. **Access Location Drop Down:** In the website's navigation section, click on the Location drop-down menu. This will display all the USA locations.
3. **Save the Webpage:** Save the HTML webpage manually.
4. **Extract URLs:** Use a Python script (`brands_scraper\scraper_scripts\hyattplace\hyattplace_script.py`) to extract all location URLs from the saved HTML page. The extracted URLs will be saved in `brands_scraper\scraper_scripts\hyattregency\hyattplace_urls.csv`.
5. **Collect Cookies and Headers:** Collect the cookies and headers from `https://www.hyatt.com/hyatt-regency/en-US/bhmhr-hyatt-regency-birmingham-the-wynfrey-hotel`.
6. **Get a Second Set of Cookies and Headers:** To avoid IP blocks after few Requests, collect a second set of cookies and headers. Use the Opera browser with an Americas or any other Region VPN enabled and revisit the URL to get this second set.
7. **Configure Main Script:** Configure both sets of collected cookies and headers in the main script located at `brands_scraper\scraper_scripts\hyattplace\main.py`.
