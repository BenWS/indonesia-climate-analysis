# About 

This project contains a set of analyses focused around data from [this](https://www.kaggle.com/datasets/greegtitan/indonesia-climate) Kaggle data source


# Pertinent Links
- [Kaggle Page](https://www.kaggle.com/datasets/greegtitan/indonesia-climate)


# Resources
 - `Data Dictionary.xlsx`
 - `climate_data.csv`

# Exploratory Analysis

<!-- 
PROJECT PLANNING: EXPLORATORY ANALYSIS
 -->

 <!-- TODO: Planning -->

<!-- TODO: Separate the column-definition activities from the analysis preparation activities in template; data preparation is an activity that could be useful for dashboarding projects -->

Copied from General Notes:

Process Steps:
- [x] Complete  `Data Dictionary.xlsx` file
  - [x] Provide column definitions for each column in provided datasets
  - [x] Identify column types in terms of qualitative or quantitative, discrete or continuous
- [ ] Identify general learning aims (just a few, nothing too extensive)
  - [ ] __General Aims__ section
  - [ ] __Analysis Implementation__ section
- [ ] Work through 'Guiding Questions` and produce analysis outline based on such
	- *An initial outline of the analysis might be beneficial to produce here. Keep such in an `Analysis/Analysis Design.md` document in project workspace*
- [ ] Determine one or two paths of further analysis for future research


__Column Definition__

*See `Data Dictionary.xlsx` for column definitions*

__Column Types__

*Identified and described in `Data Dictionary.xlsx`*

__Identify Columns for Summary Statistics__

<!-- TODO: -->

 - Range of years in data
 - Count of distinct station IDs
 - Temperature spread

__General Questions and Aims__

*Formulate some high-level conceptual questions; beneficial if these are 'testable' by the available data.*

 - Do other trends in the data (such as change in wind direction, wind speed, or rain fall over time) align with weather trends and phenomena *outside* of the context of global climate change?
 - Is global warming reflected in the monitoring station data?
 - What are the climate trends over time by station, region, and province? Do they seem to agree with the expecation?

__Analysis Outline__


<!-- 
Produce initial outline of exploratory analysis and describe in terms of dataset features (columns), summary statistics, and related visualizations. Provide limited commentary on relevance of visualization (if needed). 

Describe when the analysis outline should be considered complete...
-->

Outline:
- Introduction:
  - Goals of this analysis from an exploratory analysis standpoint
    - Identify and indicate the outliers
    - Identify quality of the data in terms of completeness
  - Trends we're looking for:
    - Seasonal trends
		- Climate change
    - Geographical trends
  - Do some statistically significant events align with historically significant events recorded on Wikipedia or generally some available reference? In the reverse, do we see recorded events apparent in the data?
- Are there any noticeable changes over time present in the results?
	- Time Series charts for
  	- Temperature (on single axes)
  		-	Minimum temperature
  		-	Maximum temperature
  		-	Average temperature
  	- Rainfall
  	- Wind speed (on single axes)
    	- Wind speed average
    	- Wind speed maximum
  	- Wind direction at maximum speed
  	- Duration of Sunshine
  	- Humidity
- Summary statistics (i.e. using df.describe() or a similar feature of Pandas)
  - What are the statistics numbers overall (see note below)?
  - What are the statistics numbers for each province?
	- What underlying stations and regions are driving the significant behavior? For example - do stations in a particular region receive more rainfall than others? 
- Correlation 
  - Is location related to (or the cause of) any outstanding or significant weather behavior? Represent such in terms of statistics and geography (if possible)
- For the more promising summary statistics (if any), represent such via either box plots and/or small multiple histograms and time series charts
- Conclusion:
  - What did this analysis confirm about our previous suppositions?
  - What results were unexpected?
  - What are some next steps we should take?
  - ...

Additional notes:
- 'Statistics' above refers to any of the following:
	- Standard statistics
		- Average
  	- Standard Deviation
  	- Maximum
  	- Minimum
  	- Count
	- Special statistics
  	- Adjusted measure of standard deviation. That is, phrased in % rather than absolute number, for easier comparison between distributions of different magnitudes.
	- Perhaps some color could be beneficial in highlighting the significant values of a given statistic?


---

Notes on 'completion' of exploratory analysis:

Exploratory analysis may be mostly about casting a wide net, meaning that we create a wide variety of statistics and plots (based on the type of data we're exploring) and then narrow the results down to the most useful information. We should go into the analysis with some idea of the information we would like to procure - however, our initial goal may evolve as we explore (which is okay).

---

Miscellaneous
 - Summary statistics for each station, region, and province, and overall
   - Average, standard deviation, minimum, and maximum for each station
 - Time Series visualizations for each region and province 
 - Map plot of country and circles visualizing the amount of rainfall each station received
 - *See physical notes box for additional thoughts, write those here*

<!-- WIP: Create Analysis Outline 
	- [ ] Determine how to treat planning of subsequent analysis and how/where such planning should be kept
	- [ ] Complete analysis outline - see comment elsewhere in section for requirements
-->

__Tableau Dashboard Opportunities__

 - Summary by Station - user selects a weather station and views summary details for station compared against full summary of all stations
 	- The temperature could be reflected in a 'thermometer visualization'
 - If station location data is perhaps available, a map indicating the location of each might be interesting (in complement with other data)
 - ...

__Produce Analysis__

<!-- TODO: -->

*Provide location of analysis here*

__Future Analysis__

<!-- TODO: -->

*Provide some additional questions and ideas for next steps here, after exploratory analysis. Having further questions is a positive sign in that the initial analysis was successful in generating thought. Establish additional high-level conceptual questions, as a sort of feedback loop to the original 'Formulate Questions' section.*