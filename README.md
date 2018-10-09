# Craigslist Filter
#### In Development...

Craigslist Filter (working title) is a web application built with python and flask which scrapes data about vehicles for sale from all Craigslist pages in America and allows users to filter them by criteria such as city, price, manufacturer, and odometer. This project is currently in development and is not yet completed.

## Installing

This application requires Python 3.6 or greater and several installable modules.

You will need to install flask, sqlite3, wtforms, lxml, and requests.

```
pip3 install Flask
```
```
pip3 install pysqlite3
```
```
pip3 install wtforms
```
```
pip3 install lxml
```
```
pip3 install requests
```

## Deploying

To run this application locally you will first need to run both crawlCities.py and scrapeVehicles.py in order to generate the databases used by the application.

Once these applications have completed, simply run app.py and copy and paste the address provided in the terminal into your browser.

## Specific Future Implementations

* The filter is operational but minor improvements are still in the works

* Pivoting to a new fancier requests module as Python's generic requests module is very slow and therefore scrapeVehicles can take many hours fully gather all the data on Craigslist (usually around a million entries).

* Login/Logout functionality which allows users to save certain filter combinations and search results.

* Scrape the map on the listing page to extract more specific location instead of just the region.

* Add some message that alerts a user when their search yields no results and remains on the form page instead of simply showing a blank results page.

## Broad Future Implementations

* Better site layout, less bootstrap-esque and more creative.

* Improved security.

* Frequent automated database updates.

* User-specific sale tracking (price has changed, listing has been removed, etc.).

* Book a domain put the application online (this could be tricky as Craigslist probably wouldn't be pleased).

## Completed Tasks

* Improved filter form including dropdown lists automatically generated by column entries in the database.

## Known Bugs

* Searching by a price/odometer of 0 is picked up as None by python and the filter is ignored.

## Contributors

This application is being developed by Austin Reese and Chris Horton.
