# **Real Estate Scraping** (_Apartment Listings in South Africa_)

A **robotic process automation (RPA)** workflow that scrapes **apartment** listing details from www.property24.com when a user provides a city name in an input dialog box.

## Step 1: Enter Location Name

Robot asks for a location name and submits.

![dialog box](web-screenshots/filled-dialog-box.png)

## Step 2: Fill Search Form

Robot opens a Google Chrome browser and enters location name in a search and hits the `enter` key. Also selects Apartment/Flat from the **Property Type** drop down,

![homepage of property24.com with search box](web-screenshots/advanced-search-box.png)

## Step 3: Scrape Structured Data

The software robot scrapes price, number of bedrooms, number of bathrooms, floor size and location data of the top 100 apartment listings from a given city in South Africa. (e.g. Cape Town). Span multiple pages to scrape the first 100 listings

![aprtment listings](web-screenshots/listings.png)

## Step 4: Save Data to Microsoft Excel

Sort and save scraped data to Microsoft Excel for further **analysis**

## Workflow

1. Enter a city name in a dialog box
2. Robot enters the name in a search box, hits the `enter` key and selects apartment/flat from the Property type drop down
3. Scrapes price, number of bedrooms, number of bathrooms, floor size and location data of the first 100 listings.
4. Sort the data table by price

TODO:

- Replicate same for real estate listings in US (Zillow, Trulia) and UK.
- Scrape all data and save to Microsoft Excel
- Analyze data in Excel
- Push data from Excel to a database.
- Create PWA with scraped data (Proof of concept).
