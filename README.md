# Project 2 - Ames Housing Data and Kaggle Challenge

### Problem Statement

In these uncertain times (2010) in the wake of the housing bubble bursting, it is more important than ever to find reliable price predictions for our properties.  Predictors we have relied on in the past may no longer hold true, as the market panic changes purchasing habits.  

In order to best serve our interests, I will design a predictive model based on the most current data, utilizing the power of machine learning to predict sale prices with the greatest precision possible.  Furthermore, I will identify 'human-readable' elements our agents can use in the field, as key points for emphasis and upselling.

---

### Data Dictionary

| name | type | description |
| - | - | - |
Id  | integer | Identifying number
Lot Frontage  | float | Linear feet of street connected to property
Lot Area  | integer | Lot size in square feet
Overall Qual  | integer | Overall material and finish quality on a scale of 1-10
Year Built  | integer | Original construction date
Year Remod/Add  | integer | Remodel date (same as construction date if no remodeling or additions)
Mas Vnr Area  | float | Masonry veneer area in square feet
Exter Cond  | integer | Present condition of the material on the exterior
Heating QC  | integer | Heating quality and condition
Gr Liv Area  | integer | Above grade (ground) living area square feet
Bsmt Full Bath  | float | Basement full bathrooms
Bsmt Half Bath  | float | Basement halfbathrooms
Full Bath  | integer | Full bathrooms above grade
Half Bath  | integer | Half bathrooms above grade
Kitchen Qual  | integer | Kitchen quality
TotRms AbvGrd  | integer | Total rooms above grade (does not include bathrooms)
Fireplaces  | integer | Number of fireplaces
Garage Cars  | float | Size of garage in car capacity
Garage Area  | float | Size of garage in square feet
Mo Sold  | integer | Month sold
Yr Sold  | integer | Year sold
SalePrice  | integer | The property's actual sale price in dollars [target variable]
| --- | --- | --- |
Lot Shape_IR  | integer | General shape of property = Slightly irregular
Lot Shape_IR3  | integer | General shape of property = Irregular
Lot Shape_Reg  | integer | General shape of property = Regular
| --- | --- | --- |
Land Contour_HLS  | integer | Flatness of the property = Hillside - Significant slope from side to side
Land Contour_Low  | integer | Flatness of the property = Depression
Land Contour_Lvl  | integer | Flatness of the property = Near Flat/Level
| --- | --- | --- |
Lot Config_CulDSac  | integer | Lot configuration = Cul-de-sac
Lot Config_FR2  | integer | Lot configuration = Frontage on 2 sides of property
Lot Config_FR3  | integer | Lot configuration = Frontage on 3 sides of property
Lot Config_Inside  | integer | Lot configuration = Inside lot
| --- | --- | --- |
Neighborhood_Blueste  | integer | Physical location within Ames city limits = Bluestem
Neighborhood_BrDale  | integer | Physical location within Ames city limits = Briardale
Neighborhood_BrkSide  | integer | Physical location within Ames city limits = Brookside
Neighborhood_ClearCr  | integer | Physical location within Ames city limits = Clear Creek
Neighborhood_CollgCr  | integer | Physical location within Ames city limits = CollegeCreek
Neighborhood_Crawfor  | integer | Physical location within Ames city limits = Crawford
Neighborhood_Edwards  | integer | Physical location within Ames city limits = Edwards
Neighborhood_Gilbert  | integer | Physical location within Ames city limits = Gilbert
Neighborhood_Greens  | integer | Physical location within Ames city limits = Greens
Neighborhood_GrnHill  | integer | Physical location within Ames city limits = Green Hills
Neighborhood_IDOTRR  | integer | Physical location within Ames city limits = Iowa DOT and Rail Road
Neighborhood_Landmrk  | integer | Physical location within Ames city limits = Landmark
Neighborhood_MeadowV  | integer | Physical location within Ames city limits = Meadow Village
Neighborhood_Mitchel  | integer | Physical location within Ames city limits = Mitchell
Neighborhood_NAmes  | integer | Physical location within Ames city limits = North Ames
Neighborhood_NPkVill  | integer | Physical location within Ames city limits = Northpark Villa
Neighborhood_NWAmes  | integer | Physical location within Ames city limits = Northwest Ames
Neighborhood_NoRidge  | integer | Physical location within Ames city limits = Northridge
Neighborhood_NridgHt  | integer | Physical location within Ames city limits = Northridge Heights
Neighborhood_OldTown  | integer | Physical location within Ames city limits = Old Town
Neighborhood_SWISU  | integer | Physical location within Ames city limits = South & West of Iowa State University
Neighborhood_Sawyer  | integer | Physical location within Ames city limits = Sawyer
Neighborhood_SawyerW  | integer | Physical location within Ames city limits = Sawyer West
Neighborhood_Somerst  | integer | Physical location within Ames city limits = Somerset
Neighborhood_StoneBr  | integer | Physical location within Ames city limits = Stone Brook
Neighborhood_Timber  | integer | Physical location within Ames city limits = Timberland
Neighborhood_Veenker  | integer | Physical location within Ames city limits = Veenker
| --- | --- | --- |
Bldg Type_2fmCon  | integer | Type of dwelling = Two-family Conversion; originally built as one-family dwelling
Bldg Type_Duplex  | integer | Type of dwelling = Duplex
Bldg Type_Twnhs  | integer | Type of dwelling = Townhouse Inside Unit
Bldg Type_TwnhsE  | integer | Type of dwelling = Townhouse End Unit
| --- | --- | --- |
House Style_1.5Unf  | integer | Style of dwelling = One and one-half story: 2nd level unfinished
House Style_1Story  | integer | Style of dwelling = One story
House Style_2.5Fin  | integer | Style of dwelling = Two and one-half story: 2nd level finished
House Style_2.5Unf  | integer | Style of dwelling = Two and one-half story: 2nd level unfinished
House Style_2Story  | integer | Style of dwelling = Two story
House Style_SFoyer  | integer | Style of dwelling = Split Foyer
House Style_SLvl  | integer | Style of dwelling = Split Level
| --- | --- | --- |
Exterior 1st_AsphShn  | integer | Exterior covering on house = Asphalt Shingles
Exterior 1st_BrkComm  | integer | Exterior covering on house = Brick Common
Exterior 1st_BrkFace  | integer | Exterior covering on house = Brick Face
Exterior 1st_CBlock  | integer | Exterior covering on house = Cinder Block
Exterior 1st_CemntBd  | integer | Exterior covering on house = Cement Board
Exterior 1st_HdBoard  | integer | Exterior covering on house = Hard Board
Exterior 1st_ImStucc  | integer | Exterior covering on house = Imitation Stucco
Exterior 1st_MetalSd  | integer | Exterior covering on house = Metal Siding
Exterior 1st_Plywood  | integer | Exterior covering on house = Plywood
Exterior 1st_Stone  | integer | Exterior covering on house = Stone
Exterior 1st_Stucco  | integer | Exterior covering on house = Stucco
Exterior 1st_VinylSd  | integer | Exterior covering on house = Vinyl Siding
Exterior 1st_Wd Sdng  | integer | Exterior covering on house = Wood Siding
Exterior 1st_WdShing  | integer | Exterior covering on house = Wood Shingles
| --- | --- | --- |
Exterior 2nd_AsphShn  | integer | Additional exterior covering on house = Asphalt Shingles
Exterior 2nd_Brk Cmn  | integer | Additional exterior covering on house = Brick Common
Exterior 2nd_BrkFace  | integer | Additional exterior covering on house = Brick Face
Exterior 2nd_CBlock  | integer | Additional exterior covering on house = Cinder Block
Exterior 2nd_CmentBd  | integer | Additional exterior covering on house = Cement Board
Exterior 2nd_HdBoard  | integer | Additional exterior covering on house = Hard Board
Exterior 2nd_ImStucc  | integer | Additional exterior covering on house = Imitation Stucco
Exterior 2nd_MetalSd  | integer | Additional exterior covering on house = Metal Siding
Exterior 2nd_Plywood  | integer | Additional exterior covering on house = Plywood
Exterior 2nd_Stone  | integer | Additional exterior covering on house = Stone
Exterior 2nd_Stucco  | integer | Additional exterior covering on house = Stucco
Exterior 2nd_VinylSd  | integer | Additional exterior covering on house = Vinyl Siding
Exterior 2nd_Wd Sdng  | integer | Additional exterior covering on house = Wood Siding
Exterior 2nd_Wd Shng  | integer | Additional exterior covering on house = Wood Shingles
| --- | --- | --- |
Mas Vnr Type_BrkFace  | integer | Masonry veneer type = Brick Face
Mas Vnr Type_None  | integer | Masonry veneer type = None
Mas Vnr Type_Stone  | integer | Masonry veneer type = Stone
| --- | --- | --- |
Foundation_CBlock  | integer | Type of foundation = Cinder Block
Foundation_PConc  | integer | Type of foundation = Poured Concrete
Foundation_Slab  | integer | Type of foundation = Slab
Foundation_Stone  | integer | Type of foundation = Stone
Foundation_Wood  | integer | Type of foundation = Wood
| --- | --- | --- |
Central Air_Y  | integer | Central air conditioning
| --- | --- | --- |
Paved Drive_P  | integer | Paved driveway = Partial
Paved Drive_Y  | integer | Paved driveway = Paved
| --- | --- | --- |
Sale Type_CWD  | integer | Type of sale = Warranty Deed - Cash
Sale Type_Con  | integer | Type of sale = Contract 15% Down payment regular terms
Sale Type_ConLD  | integer | Type of sale = Contract Low Down
Sale Type_ConLI  | integer | Type of sale = Contract Low Interest
Sale Type_ConLw  | integer | Type of sale = Contract Low Down payment and low interest
Sale Type_New  | integer | Type of sale = New Home just constructed and sold
Sale Type_Oth  | integer | Type of sale = Other
Sale Type_WD  | integer | Type of sale = Warranty Deed - Conventional

---

### Methodology

I used initial EDA to narrow the available features from 81 to 35.  Applying a Linear Regression model to these features, I used scikit metrics to assess its performance on training and test data.

---

### Summary of Findings

While overall real estate sales have declined, the price point of individual sales has only changed slightly.  Focusing on quality of sales over quantity is a winning strategy in the current market.

---

### Conclusions / Recommendations

#### Conclusions: 
There is a lot to say here, but I'll try to distill key points.

* Contract sales with 15% down and regular terms closed at a whopping \$43,731 above the mean, holding all else equal.  
* Low down payment, low interest contract sales were also notable, at \$30,670 above, holding all else equal.
* 2.5 story finished buildings sold at markedly higher prices than other types, at \$62,690 above.  No other type even came close to such a large difference from the mean.
* Hard material exteriors are a strong indicator of sale price.  Brick Face (NOT Common) and Stone primary exteriors showed sale prices of \\$20,254 and \\$19,291 above the mean, holding all else equal.  Cement Board was an even more pronounced indicator, at \$42,697.
* Each car the garage holds can be expected to increase sale price by \$6,113.81, holding all else equal.
* Neighborhood may be the influence on sale price of all.  In descending order, Green Hill, Stonebridge, and Northridge Heights properties closed at the highest prices relative to other factors, reaching nearly \$100,000 for properties in Green Hill.
* Most neighborhoods had a much less significant impact on final price, but Edwards and Old Town were among the worst, both at approximately \$30,000 below mean, holding all else equal.
* Holding all else equal, properties yield approximately $77.20 dollars less for each year elapsed since construction.
* Renovations, interestingly, had a greater impact on overall sale price, at \$131.97 per year.

#### Recommendations:  

* Acquire properties in less desirable neighborhoods as long term investments.
* Focus on contract sales and new construction sales.  Cash sales are expected to yield lower final prices.
* Finished, larger dwellings add a great deal of value.  Investment in a little bit of work and furnishing can yield considerable profits on the final sale.

---

### Kaggle Submission

https://www.kaggle.com/c/dsir-202021214-w-project-2-regression-challenge/

Score: 31249.08207

