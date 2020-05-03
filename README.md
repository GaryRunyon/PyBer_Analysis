# PyBer_Analysis

This exploratory data analysis was conducted to identify and visualize trends in ride data, in order to help improve access to ride sharing services and improve affordability in under-served neighborhoods. Once the data was loaded and inspected, it was then stratified according to city type. This allowed for the calculation of summary statistics such as total number of rides, total number of drivers, average fare per ride, average fare per driver, etc. The Summary Data Frame clearly shows an excess of drivers in urban areas, where fares are the lowest, and a scarcity of drivers in rural areas, where fares are the highest. The line chart provided supported this disparity in fares while showing a similar pattern for all three city types: peak revenue toward the end of February with predictable and consistent fluctuations until the beginning of May, the end of the collection period. 


The rate-limiting component of the analysis was the stratification of data into groups based on “city type.” Generally speaking, however, there were no difficulties analyzing the data, as the data extracted/ loaded was clean, well-formatted, and absent of any anomalous values. Had this not been the case, simple tools to find missing data [e.g. count( ), isnull( ), notnull(  )], handle erroneous values [e.g. dropna( ), fillna( )] or change inconsistent data types [e.g. astype( ), _to_(datatype)] could have been quickly used to normalize the dataset. 





In summary, I believe the data to suggest the following actions. In order to achieve the primary endpoint of improving affordability and accessibility in underserved neighborhoods, more drivers and cheaper fares are needed in rural areas whereas fewer drivers and higher fares would be prudent in urban areas. There are other measures outside the scope of the data provided that would also be useful. Start tracking “Wait Times” (measured as “time_stamp_ride_begins” - “time_stamp_ride_requested”) and “Ride Capture” (measured as “number_of_rides_executed“ / “number_of_rides_requested” * 100). Plot the data to ascertain whether or not a correlation exists between wait times and cancellation percentage, the inverse of ride capture. This would be an excellent indicator of the need to hire additional drivers. Begin tracking customer satisfaction via “Py-Rating.” This would assist in recognizing and rewarding positive performance while identifying and improving negative performance. In most customer-driven business models, there is a direct correlation between customer satisfaction, brand loyalty and revenue trends. Additionally, increasing the sample size of data, to 2 years or more, would help establish seasonality. This could enhance profitability by having more drivers available when demand increases and less drivers on payroll when demand retracts.
