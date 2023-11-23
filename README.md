**Project Title:** City Locator

**Overview:** 

Cities Locator is a Python-based geographical analysis tool designed to empower users in discovering the closest cities to a specified coordinate, while allowing for population-based filtering. Leveraging sophisticated algorithms such as Haversine and Vincenty, the program ensures precise latitude and longitude distance calculations, with automatic algorithm fallback to guarantee reliable results. The main part of the code is the Cities class, an object-oriented solution that efficiently manages city data, encapsulating vital information like name, latitude, longitude, and population. The command-line interface, powered by argparse, provides a seamless user experience, enabling customization of inputs, including the file path to city data, reference coordinates, minimum population thresholds, and the desired number of results. Users can harness the program's capabilities by providing a data file in a tab-delimited format, such as the provided city_data.txt. This file structure allows for easy adaptation to different datasets, offering versatility in city analysis


**Usage**

Installation: Ensure dependencies are installed by running:
python3 -m pip install --upgrade pip
python3 -m pip install haversine vincenty

Ensure to download the following sample data file to directory:

city_data.txt



**Running the code: Execute the program by providing the necessary command-line arguments:**

python3 cities.py city_data.txt 38.9897 -76.9378
python3 cities.py city_data.txt 38.9897 -76.9378 -p 50_000
python3 cities.py city_data.txt 38.9897 -76.9378 -n 5
python3 cities.py city_data.txt 38.9897 -76.9378 -p 50_000 -n 5
