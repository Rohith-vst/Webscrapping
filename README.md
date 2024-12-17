Car Specifications Scraper 🚗


Project Description
This project is a web scraper built to extract car model specifications, variants, prices, and other details from automotive websites like CarWale. The scraper collects data such as engine specifications, dimensions, safety features, fuel efficiency, and pricing, then organizes it into a structured CSV file for analysis or comparison.

The project leverages Python, BeautifulSoup, and Pandas to fetch, parse, and store the data.

Features
Dynamic Scraping:

Scrapes all car models and their variants for a selected car brand.
Fetches technical specifications (engine, dimensions, mileage, etc.) for each variant.
Organized Data Output:

Saves the data into a clean CSV file.
Suitable for further data analysis or visualization.
Robust Error Handling:

Handles invalid URLs, missing fields, or failed network requests gracefully.
Easy Customization:

Modify the brand_url to scrape different car brands.
Tech Stack
Python 3.8+
Requests (for HTTP requests)
BeautifulSoup4 (for HTML parsing)
Pandas (for data organization and saving CSV files)
Dataclasses (for structured storage of car details)

The requirements include:

requests

beautifulsoup4

pandas

Usage

Run the Script
To scrape data for a specific car brand (e.g., Mahindra), execute the script:

bash

python car_scraper.py
Customize for Other Brands
Update the brand_url variable in the script with the desired car brand's page URL from CarWale.
Example:

python

brand_url = "https://www.carwale.com/mahindra-cars/"
Output
The scraped data will be saved in a CSV file named:


Key Functions
scrape_all_cars(brand_name, brand_url):

Scrapes all car models and their variants for a specific brand.
fetch_variants(car_link):

Fetches all the variants, prices, and links for a specific car model.
scrape_variant_details(brand_name, car_name, variant_name, variant_link):

Scrapes specifications of a specific car variant.
safe_find(data_itemid):

Safely extracts specific car details from the HTML content.

**Possible Applications**

Automotive Comparisons: Compare specifications, features, and prices of various car models.

Market Research: Analyze trends in fuel efficiency, engine specifications, or safety ratings.

Data Visualization: Use tools like Excel, Tableau, or Power BI to visualize the scraped data.

Consumer Insights: Help buyers make informed decisions based on technical specifications.

Known Limitations
The scraper is specifically designed for CarWale.com and may not work on other automotive websites without adjustments.

Some variants or specifications might be unavailable due to website structure or incomplete data.

**Future Improvements**

Add support for other car websites or multiple brands in a single run.

Implement multi-threading to improve scraping efficiency.

Integrate a database to store and manage scraped data.

Include a web dashboard for real-time data visualization.

Contributing

Contributions are welcome! Follow these steps to contribute:

Fork the repository.
Create a new branch (feature/your-feature-name).
Commit your changes and push to your branch.
Submit a pull request.
License
This project is licensed under the MIT License.

Contact
For any issues or suggestions, feel free to contact me at:

Email: rohiththammu@gmail.com
GitHub: https://github.com/Rohith-vst
Happy Scraping! 🚀
