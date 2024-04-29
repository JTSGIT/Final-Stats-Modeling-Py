## Project/Goals
The goal of this project is to explore the relationship between the availability of free bikes and the characteristics of points of interest (POIs) in Barcelona using data from Foursquare and YELP API. Specifically, I aimed to build a regression model to predict the number of free bikes available at various locations based on the number and ratings of nearby POIs.

## Process

### Data Collection
Data was collected from two main sources:
- **Bike Stations**: Data on bike stations including the number of free bikes was collected via the CityBikes API.
- **POIs**: Data on nearby POIs was gathered using the Foursquare and Yelp APIs, focusing on the proximity of restaurants and other attractions to each bike station.

### Data Preparation and Analysis
- **Data Cleaning**: The data was cleaned to handle inconsistencies and missing values. Latitude and longitude data were used to calculate distances.
- **Feature Engineering**: New features such as the distance to the nearest restaurant were calculated using the Haversine formula.
- **Regression Analysis**: A linear regression model was built to explore how the number of nearby POIs and their ratings relate to bike availability.

## Results
The regression analysis revealed that:
- There is a significant relationship between the proximity of high-rated restaurants and bike availability.
- Bike stations closer to popular restaurants tend to have fewer available bikes, likely due to higher usage rates.

## Challenges 
The main challenges faced during the project included:
- Handling missing data from the APIs, which required careful data imputation strategies.
- Dealing with multicollinearity in the regression model due to closely related geographic features.
- Ensuring enough data was available for robust statistical analysis, as the sample size was relatively small.

## Future Goals
With more time, I would:
- Expand the dataset to include more bike stations and a broader range of POIs to enhance model accuracy.
- Incorporate additional variables such as weather conditions and temporal factors (time of day, day of the week) that might affect bike usage.
- Apply more complex models and machine learning techniques to improve predictions and provide more dynamic insights.

