# Chennai House Price Prediction

## Problem Statement
1. Real estate transactions are quite opaque sometimes and it may be difficult for a newbie to know the fair price of any given home. Thus, multiple real estate websites have the functionality to predict the prices of houses given different features regarding it. Such forecasting models will help buyers to identify a fair price for the home and also give insights to sellers as to how to build homes that fetch them more money. 
2. Chennai house sale price data is presented in train-chennai-sale.csv file and we try to build a sale price prediction model that will aid the customers to find a fair price for their homes and also help the sellers understand what factors are fetching more money for the houses.


Based on the train dataset, we need to develop a model that accurately predicts the real estate price in Chennai.

## House Features:

	• INT_SQFT – The interior Sq. Ft of the property 
	• N_BEDROOM – The number of Bed rooms 
	• N_BATHROOM - The number of bathrooms 
	• N_ROOM – Total Number of Rooms 
	• QS_ROOMS – The quality score assigned for rooms based on buyer reviews
	• QS_BATHROOM – The quality score assigned for bathroom based on buyer reviews 
	• QS_BEDROOM – The quality score assigned for bedroom based on buyer reviews 
	• QS_OVERALL – The Overall quality score assigned for the property 
	• SALE_COND – The Sale Condition Normal: 
		○ Normal Sale 
		○ Abnorml: Abnormal Sale - trade, foreclosure, short sale 
		○ AdjLand: Adjoining Land Purchase 
		○ Family: Sale between family members 
		○ Partial: Home was not completed when last assessed 
	• BUILDTYPE – The type of building House Commercial Others Surrounding and Locality
	• AREA – The property in which the real estate is located 
	• DIST_MAINROAD – The distance of the property to the main road 
	• PARK_FACIL – Whether parking facility is available 
	• UTILITY_AVAIL
		AllPub: All public Utilities (E,G,W,& S)
		NoSewr: Electricity, Gas, and Water (Septic Tank)
		NoSeWa: Electricity and Gas Only
		ELO: Electricity only 
	• STREET
		Gravel
		Paved
		No Access 
	• MZZONE
		A: Agriculture
		C: Commercial
		I: Industrial
		RH: Residential High Density
		RL: Residential Low Density
		RM: Residential Medium Density
	• PRT_ID – The Property Transaction ID assigned by ChennaiEstate
	• COMMIS – The Commission paid to the agent
	• SALES_PRICE – The total sale price of the property
	 
## Contents

	1. Import Libraries
	2. Read Data
		a. Observation
			i. Shape, Describe, Info, Null
	3. Text Pre-processing
		a. General Data Cleaning
			i. Fill Null columns
			ii. Change data type of columns
			iii. Drop PRT_ITEMS
		b. Column by Column Cleaning
			i. Area
			ii. N Bed, Bath, Rooms
			iii. Sale condition
			iv. Park facility
			v. Build type
			vi. Utility avail
			vii. Street
			viii. Mzzone
			ix. Reg fee & Commis
			x. Date of sale & build
	4. Feature Engineering
		a. House age
		b. Dimentionality reduction
			i. Correlation graph
			ii. All QS features
			iii. DIST_MAINROAD
			iv. REG_FEE & COMMIS
			v. N_ROOM
		c. Encoding
			i. Ordinal
			ii. Nominal
		d. Feature Selection
		e. Dropping coloumns
		f. Outliers
	5. Exploratory Data Analysis
		a. Categorical feature analysis
			i. Area
			ii. N Bed, Bath, Rooms
			iii. Sale condition
			iv. Park facility
			v. Build type
			vi. Utility avail
			vii. Street
			viii. MZ ZONE
		b. Continous feature analysis
			i. Sales price
			ii. INT_SQFT
			iii. House age
	6. ML Models
		a. Linear Regression
			i. Feature Importance Graph
			ii. Prediction Analysis
		b. XG Boost
			i. Feature Importance Graph
			ii. Prediction Analysis
		c. Random Forest
			i. Feature Importance Graph
			ii. Prediction Analysis
		d. Decision Tree
			i. Feature Importance Graph
			ii. Prediction Analysis
	7. Conclusion
		a. Important Features
		b. User Specific Prediction
		c. Observation




