# SimpliPlan

SimpliPlan is a Financial Application with three different main functions namely:
1. Financial Planning
2. Calculate Car Affordability
3. Calculate Housing Affordability

Basic Front-End was designed with HTML5, CSS and JavaScript using BootStrap
Backend was implemented with Django


# To Start:
run the following in the command line: manage.py migrate --run-syncdb

Load resale flat prices by running the following in the command line:
sqlite3.exe db.sqlite3
.mode csv
.import House/resale-flat-prices-2021.csv House_resaleflatprice

Load Car and Fuel Prices by running the following in the command line:
python manage.py loadCar Car/cars.csv
python manage.py loadFuel Car/fuel.csv

Create your own superuser:
python manage.py createsuperuser

Start the application:
python manage.py runserver

# Disclaimer:
Prices of car, fuel and housing are just for example and may not be accurate.
Certain formulas may not be applicable depending on country of residence.
