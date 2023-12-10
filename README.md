# Models, Makes and Accident Rates: A Summary.
## What Makes a Flight Safe?

In the dynamic world of aviation, the acknowledgment that complete risk elimination is challenging sets the stage for our exploration. The focus of this project lies in strategies aimed at minimizing risk by prioritizing passenger safety. The critical importance of passenger safety in the decision-making process is duly recognized, given the potential severe repercussions a fatal accident could inflict on a company's reputation and financial stability.

The analysis is designed to offer recommendations on three key aspects:

1. Makes and models of airplanes with the lowest percentages of injuries

2. Engine type and number of engines and whether or not it contributes to safety using the data provided

3. Weather conditions and how they contribute to accident rates

While recognizing that other factors contribute to flight safety, these aspects are deemed pivotal for our assessment.

 ## The Dataset: Unveiling Insights from 1948 to 2023

The dataset, provided by the 'National Transportation Safety Board,' spans aviation accident data from 1948 to 2023. Our primary focus is on data from 1981 to 2023, as earlier data offers limited insights into fatality rates.

 ## Navigating the Dataset: Tools and Insights

We begin by leveraging essential tools:

Pandas: To read and manipulate the dataset.
Numpy: For data manipulation and filtering (termed as "cleaning").
MatPlotLib: For visualization.
MatPlotLib Inline: For displaying interactive plots directly in the cells.

An initial observation reveals that several columns are missing well over 1000 rows of data. To address this, we opt to drop unnecessary columns and clean up rows.

 ## Dropping Unnecessary Columns

Given the dataset's size, columns missing more than half of their data are considered for removal. The columns identified for elimination include 'Latitude,' 'Longitude,' 'Aircraft.Category,' 'FAR.Description,' 'Schedule,' and 'Air.carrier.'

Additionally, other flight-specific columns, such as 'Accident.Number,' 'Registration.Number,' 'Report.Status,' 'Publication.Date,' 'Airport.Code,' 'Airport.Name,' and 'Purpose.of.Flight,' are deemed non-essential for our research and are dropped.

 ## Cleaning Make and Model: A Prerequisite for Analysis

The pivotal role of makes, models, and aircraft types necessitates thorough cleaning. A new column, 'Make.and.Model,' is created to facilitate comparison and filling in missing values. Unnecessary rows, including those not related to airplanes, are removed.

 ## Passengers Injured and Aircraft Damage: Ensuring Comprehensive Analysis

The next focus is on passengers injured and aircraft damage. We delve into finding missing data, calculating total passengers on each flight, and creating new columns for comprehensive insights.

Unknown values are filled to address incomplete entries. The analysis extends to understanding the relationship between injury severity and aircraft damage.

 ## Unknown Fillers: Addressing Unseen Variables

Certain columns with unknown values, such as 'Location and Country' and 'Amateur Built,' are filled in with 'Unknown.' While not crucial, these entries may contribute as outliers or essential data completions.

 ## Weather Conditions and Broad Phase of Flight: Navigating Unpredictability

Assigning 'Unknown' to NaN values in 'Weather.Condition' and 'Broad.phase.of.flight,' we then explore the influence of weather conditions on accidents. A specific focus is placed on accidents occurring in Instrument Meteorological Conditions (IMC) and Visual Meteorological Conditions (VMC).

 ## Engines and Their Effect: Decoding the Impact

Understanding the effect of engines on flight safety is paramount. A closer look reveals insights into engine types, specifically highlighting the prevalence of 'Reciprocating' engines with the highest usage and fatality rates.

 ## Recommendations: Closing Statemnet

Based on our analysis, the top three aircraft with the least damage and fatality rates are:

1200 G103
MADSEN LANCAIR 320
MADSEN RANS S-12

However, considering flight frequency, the top three aircraft are:

BOEING 737
BOEING 777
BOEING 767
Noteworthy is the CESSNA 152, with over 5 million crashes but a comparatively low fatality rate, making it a subject for further consideration.

In conclusion, this analysis serves as a comprehensive guide, offering valuable insights into aviation safety based on data-driven observations. Graphical representations in Tableau further enhance our understanding, providing a visual summary of the findings
![Dashboard 2 (2)](https://github.com/Arisulo/dsc-Model-Makes-AccidentRates/assets/145289186/ac8ad356-79ae-46bc-8ab2-a9f73764b89b)
