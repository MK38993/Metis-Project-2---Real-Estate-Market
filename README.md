# Predicting New York City Housing Prices

#### Matthew Kwee, Aug. 2021

## Abstract



For this project, I constructed a Linear Regression model in order to accurately predict New York City housing real-estate prices.

Using a basic web-crawler, I scraped 9899 listings from [realtor.com](https://realtor.com"......") and trained my model from the data, which I then packaged into a function in order to predict real-estate prices.


## Design
This project presents a series of plots that highlight stations with high foot traffic, and those which have recovered from COVID lockdowns the fastest.


## Data
I scraped 9899 datapoints from [realtor.com](https://realtor.com"......"). I selected 10 features to model for each datapoint, of which 4 are categorical. Only about 850 datapoints had all 10 features available. Using the Google Maps geocoding API, I was able to fill in missing 'borough' and 'neighborhood' information, which allowed me to 'save' another ~90 datapoints. 


## Algorithms
1. Constructing a web-crawler to catalog 9900 links to listings, then scrape those listings.

2. Using the Google Maps geocoding API to fill in datapoints missing 'borough' and 'neighborhood' features, based on listing address.

3. Running Linear, Ridge, Lasso, and Elastic Net regressions on usable data, selecting the best model (the Ridge model had the highest r<sup>2</sup> value), and using it to predict housing prices.

### Models

I tested Linear, Lasso, Ridge, and Elastic-Net Regressions, but decided on Linear Regression, since my test set was not overfit - my training and test sets had similar r<sup>2</sup> values.

## Tools
- Selenium for scraping 9900 listings.

- Google Maps Geocoding API to fill in missing 'neighborhood' and 'borough' fields in listings.

- Pandas and NumPy for data manipulation.

- Scikit-Learn for creating and training regression models.

- Matplotlib and Seaborn for visualizing data.





