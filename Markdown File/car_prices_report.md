# Car Prices

## Introduction

The goal of this project is to analyze a car prices dataset and understand the factors that influence vehicle selling prices. The analysis includes data cleaning, preprocessing, exploratory data analysis, visualization, and interpretation of results.

## Dataset Overview

The dataset contains information about vehicles such as:

* Manufacturing year
* Brand
* Model
* Body type
* Vehicle Identification Number(VIN)
* Transmission
* Condition
* Odometer reading
* Manheim Market Report(MMR) value
* Selling price
* Sale date
* State

## Data Cleaning

Several cleaning steps were performed:

* Removed the VIN column because it was not useful for analysis.
* Renamed columns to make them easier to understand.
* Handled missing values in multiple columns.
* Replaced missing transmission values with "unknown".
* Fixed body type values.
* Fixed brand names and inconsistencies.
* Removed records where manufacturing year was greater than sale year.
* Converted the sale date column to datetime format.
* Created additional date-related columns such as sale year, sale month, and sale day.
* Checked for duplicate records.
* Saved the cleaned dataset for further analysis.

## Missing Value Analysis

Missing values were found in several columns.

Different techniques were used depending on the column:

* Some missing values were filled with suitable values such as "unknown".
* Missing numerical values were handled appropriately.
* Rows with important missing information were removed when necessary.

## Exploratory Data Analysis

### Total Revenue Generated

The total revenue generated from vehicle sales was calculated to get an overall idea of the sales volume.

### Selling Price Distribution

A histogram was used to study the distribution of selling prices.

Observation:

* Most vehicles were sold at lower to medium price ranges.
* A small number of vehicles had very high selling prices.

### Brand Distribution

A count plot was used to identify the most common brands.

Observation:

* Some brands appeared much more frequently than others.

### Body Type Distribution

A count plot was created for body types.

Observation:

* SUVs, sedans, and other common vehicle categories dominated the dataset.

### Transmission Distribution

Observation:

* Automatic vehicles were more common than manual vehicles.

### Manufacturing Year Distribution

Observation:

* Most vehicles were relatively recent models.

### Year with Most Sales

A count plot was used to see how sales were distributed across years.

Observation:

2015 year recorded higher sales compared to other.

## Descriptive Statistics

Descriptive statistics were generated using the describe() function.

The analysis provided:

* Mean values
* Median values
* Minimum values
* Maximum values
* Standard deviation

## Outlier Detection

Box plots were used to identify outliers in:

* Selling Price
* Maheim Market Report(Manheim Market Report(MMR)
* Odometer Reading
* Vehicle Age

A large number of outliers were observed in selling price and Maheim Market Report(MMR)  .

During check, several vehicles had an odometer reading of 999999.

This value appeared repeatedly and was treated as an invalid value rather than a real value. It was replaced using the median odometer reading.

## Correlation Analysis

A correlation heatmap was created using:

* Selling Price
* Maheim Market Report(MMR) 
* Odometer Reading
* Manufacturing Year
* Vehicle Age

Observation:

* Maheim Market Report(MMR) showed a strong positive relationship with Selling Price.
* Vehicle Age showed a negative relationship with Selling Price.
* Odometer Reading also showed a negative relationship with Selling Price.

## Feature-wise Analysis

### Vehicle Age vs Selling Price

Observation:

* Older vehicles generally sold for lower prices.

### Odometer Reading vs Selling Price

Observation:

* Vehicles with higher mileage tended to have lower selling prices.

### Maheim Market Report(MMR) vs Selling Price

Observation:

* Vehicles with higher Maheim Market Report(MMR) values generally had higher selling prices.

### Brand vs Selling Price

Observation:

* Some premium brands showed higher selling prices compared to regular brands.

### Body Type vs Selling Price

Observation:

* Vehicle prices varied across body types.

### State vs Selling Price

Observation:

* Vehicle prices showed noticeable variation across different states.

## Visualizations

The following visualizations were created:

* Histograms
* Count plots
* Scatter plots
* Box plots
* Correlation heatmap

## Key Findings

* Maheim Market Report(MMR) is strongly related to vehicle selling price.
* Older vehicles generally sell for lower prices.
* Higher mileage vehicles tend to have lower resale value.
* Automatic transmission vehicles are more common than manual vehicles.
* Vehicle prices vary across brands, body types, and states.
* Invalid odometer reading values such as 999999 were identified and corrected.

## Business Insights / Recommendations

* Maheim Market Report(MMR) can be used as an important indicator when estimating vehicle selling prices.
* Vehicle age and mileage should be considered carefully during pricing.
* Dealers can use brand and body type information to better understand market value.
* Data quality checks should be performed to identify placeholder values such as 999999.

## Conclusion

This project involved cleaning, preprocessing,analyzing and visualizing a car prices dataset. The analysis showed that factors such as Maheim Market Report(MMR), vehicle age, mileage, brand, and body type influence selling price. The dataset was successfully cleaned and explored and also provided useful insights 
