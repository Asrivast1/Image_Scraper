# Image_Scraper
This is a script made to aid in the creation of datasets (images only)for any Machine Learning program based on web scraping
using Python Script. It makes use of various packages like selenium, hashlib and PIL especially Image and other packages like
time etc. It works in steps, firstly it makes requests to fetch image urls through web which include building the google query, 
loading the page and extract image urls. The fetch_image_urls function has a try and except block to ensure that only the image
thumbnail that has an actual image behind it is downloaded, thumbnails failing the above criteria are skipped. The presence of
chromedriver is essential for this script to run, in windows generally it's present ut needs to be downloaded externally in case
of mac or Linux Derivatives OS. In the search_and_downloads functions in number_images parameter you need to specify the number
of images that you need to download. At the last of the script you need in DRIVER_PATH update the path of your chromedriver and 
in the function calling of search_and_downloads function at last of the script in the search_term parameter specify the keyword 
required for searching through the web and downloading.

Once all of this done, this script is ready to scrape through web downloading images for you. If any suggestion to make this 
script more efficient, please do feel free to commit to this repository.
