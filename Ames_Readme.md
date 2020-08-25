# Project 2: Ames Housing - Readme

## Executive Summary

This exercise examines the effects of features on the prediction of a house pricing model in the city of Ames, Iowa.

Using historical housing sale data, we are tasked to optimise the price prediction model with features that could help explain the sale value. 


Contents:
- 1.0 Data Cleaning
- 2.0 Exploratory Data Analysis
- 3.0 Preprocessing and Feature Engineering
- 4.0 Modeling Benchmarks
- 5.0 Prepare Test Set for Modeling
- 6.0 Model on Test Set
- 7.0 The Ames Housing Project Report 


Data:
- The Ames Housing Data

Using the results from our model we know that it the following coefficients have a large impact on how the price is being predicted.

We may narrow value-added features these down into 3 groups of interest:

1. Quality
2. Total Area (Sqft)
3. Neighbourhood

However, this model may not generalise well to other cities as these features are specifically unique to this area and property market. To generalise the model, we would have to underfit it which will have a negative impact on its accuracy, but increase the generalisation and decrease the bais of the model.


### Conclusion & Recommendations


Using the results from our model we know that it the following coefficients have a large impact on how the price is being predicted. 

We may narrow value-added features these down into 3 groups of interest:
1. Quality
2. Total Area (Sqft)
3. Neighbourhood


1. Quality
We can see that Quality and its permutations in the data has a large weight in the predictions. It shows that Buyers are willing to pay top dollar for houses which are built with quality in mind. The resonates with the quality of other assets on the property. 

Sellers should then focus on improving the quality of their house since they will not be able to change its location, or totsl area easily. 

2. Total Area(Sqft)
As we can expect to pay more for a larger cake, we should expect same with buying land. Although we can see that it has a large impact in the value, the negative impact of poor quality in a poorly valued neighbourhood will reverse the incremental increase in price given the area.

3. Neighbourhood
We can see from the EDA that some neighbourhood clearly have higher valued lots. We do not know the exact causation to how the neighbourhood is valued, more data is needed here. The top 3 neighbourhoods with the highest median sale price are: Stone Brook, Northridge and Northridge Heights. 


Conversely, it is suggested that poorly constructed, aesthetically poor or unfinished houses often receive lower values. 

However, this model may not generalise well to other cities as these features are specifically unique to this area and property market. To generalise the model, we would have to underfit it which will have a negative impact on its accuracy, but increase the generalisation  and decrease the bais of the model. 

#### Data Dictionary :

|Feature|Dataset|Description|
|---|---|---|
MSSubClass|Train/Test|The building class|
MSZoning|Train/Test| Identifies the general zoning classification of the sale.|
LotFrontage|Train/Test| Linear feet of street connected to property|
LotArea|Train/Test| Lot size in square feet|
Street|Train/Test| Type of road access to property|
Alley|Train/Test| Type of alley access to property|
LotShape|Train/Test| General shape of property|
LandContour|Train/Test| Flatness of the property|
Utilities|Train/Test| Type of utilities available|
LotConfig|Train/Test| Lot configuration|
LandSlope|Train/Test| Slope of property|
Neighborhood|Train/Test| Physical locations within Ames city limits|
Condition1|Train/Test| Proximity to main road or railroad|
Condition2|Train/Test| Proximity to main road or railroad (if a second is present)|
BldgType|Train/Test| Type of dwelling|
HouseStyle|Train/Test| Style of dwelling|
OverallQual|Train/Test| Overall material and finish quality|
OverallCond|Train/Test| Overall condition rating|
YearBuilt|Train/Test| Original construction date|
YearRemodAdd|Train/Test| Remodel date (same as construction date if no remodeling or additions)|
RoofStyle|Train/Test| Type of roof|
RoofMatl|Train/Test| Roof material|
Exterior1st|Train/Test| Exterior covering on house|
Exterior2nd|Train/Test| Exterior covering on house (if more than one material)|
MasVnrType|Train/Test| Masonry veneer type|
MasVnrArea|Train/Test| Masonry veneer area in square feet|
ExterQual|Train/Test| Exterior material quality|
ExterCond|Train/Test| Present condition of the material on the exterior|
Foundation|Train/Test| Type of foundation|
BsmtQual|Train/Test| Height of the basement|
BsmtCond|Train/Test| General condition of the basement|
BsmtExposure|Train/Test| Walkout or garden level basement walls|
BsmtFinType1|Train/Test| Quality of basement finished area|
BsmtFinSF1|Train/Test| Type 1 finished square feet|
BsmtFinType2|Train/Test| Quality of second finished area (if present)|
BsmtFinSF2|Train/Test| Type 2 finished square feet|
BsmtUnfSF|Train/Test| Unfinished square feet of basement area|
TotalBsmtSF|Train/Test| Total square feet of basement area|
Heating|Train/Test| Type of heating|
HeatingQC|Train/Test| Heating quality and condition|
CentralAir|Train/Test| Central air conditioning|
Electrical|Train/Test| Electrical system|
1stFlrSF|Train/Test| First Floor square feet|
2ndFlrSF|Train/Test| Second floor square feet|
LowQualFinSF|Train/Test| Low quality finished square feet (all floors)|
GrLivArea|Train/Test| Above grade (ground) living area square feet|
BsmtFullBath|Train/Test| Basement full bathrooms|
BsmtHalfBath|Train/Test| Basement half bathrooms|
FullBath|Train/Test| Full bathrooms above grade|
HalfBath|Train/Test| Half baths above grade|
Bedroom|Train/Test| Number of bedrooms above basement level|
Kitchen|Train/Test| Number of kitchens|
KitchenQual|Train/Test| Kitchen quality|
TotRmsAbvGrd|Train/Test| Total rooms above grade (does not include bathrooms)|
Functional|Train/Test| Home functionality rating|
Fireplaces|Train/Test| Number of fireplaces|
FireplaceQu|Train/Test| Fireplace quality|
GarageType|Train/Test| Garage location|
GarageYrBlt|Train/Test| Year garage was built|
GarageFinish|Train/Test| Interior finish of the garage|
GarageCars|Train/Test| Size of garage in car capacity|
GarageArea|Train/Test| Size of garage in square feet|
GarageQual|Train/Test| Garage quality|
GarageCond|Train/Test| Garage condition|
PavedDrive|Train/Test| Paved driveway|
WoodDeckSF|Train/Test| Wood deck area in square feet|
OpenPorchSF|Train/Test| Open porch area in square feet|
EnclosedPorch|Train/Test| Enclosed porch area in square feet|
3SsnPorch|Train/Test| Three season porch area in square feet|
ScreenPorch|Train/Test| Screen porch area in square feet|
PoolArea|Train/Test| Pool area in square feet|
PoolQC|Train/Test| Pool quality|
Fence|Train/Test| Fence quality|
MiscFeature|Train/Test| Miscellaneous feature not covered in other categories|
MiscVal|Train/Test| $Value of miscellaneous feature|
MoSold|Train/Test| Month Sold|
YrSold|Train/Test| Year Sold|
SaleType:|Train/Test| Type of sale|
SalePrice|Train/Test| the property's sale price in dollars.|

#### Sources:

Ames, Iowa. (n.d.). Retrieved June 11, 2020, from http://www.city-data.com/city/Ames-Iowa.html
Ames IA APPRECIATION RATE TRENDS AND HOUSING MARKET DATA. (n.d.). Retrieved June 11, 2020, from https://www.neighborhoodscout.com/ia/ames/real-estate
Ames Real Estate Forecast, Housing Market Prediction: Up to 239032 USD! - Ames City Real Estate Market Forecast 2020-2030, Long-Term &amp; Short-Term Property Home Price Prediction with Smart Technical Analysis. (n.d.). Retrieved June 11, 2020, from https://walletinvestor.com/real-estate-forecast/ia/story/ames-housing-market