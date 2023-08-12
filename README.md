# Flight_Delay_Prediction
Flight delay Analysis and Prediction

With numerous factors influencing it, air travel is becoming more and more difficult. One of these factors, the flight delay, has an influence on the airline, the airport, and the passenger. It may cause serious financial loss or harm to everyone involved, with large economic costs as a result. Therefore, anticipating delays is essential from the perspective of the customer, the carrier, and time management in order to maintain customer confidence, as well as from the airport’s perspective in order to manage traffic more effectively and maximize the number of arriving flights through timely schedule adjustments. The very significant cause of these delays has been found as the influence of the weather. 

In order to take the necessary corrective and preventive actions to improve business and service, it is in the best interest of one of the ecosystem participants to predict flight delays based on the flight details and forecasted weather conditions using a good predictive model, which you are going to build.  
Data scientists can forecast whether a delay will occur or not using flight data and aviation weather data for a specific aircraft utilizing previous data that includes scheduled departure and arrival times, date, origin, and destination as well as weather data.

# Objective
1. To derive the Categorical Target Attribute “FlightDelayStatus” for Train.csv.
2. To predict the flight delay  of each id categorizing into “1”  or  ”2”
   “1” indicates :  “Yes”  and 
   “2” indicates  : ”No”
   
Note:If the delay is more than  15 minutes then FlightDelayStatus will be “1” else “2”.

# Data
Every flight is tracked in accordance with its scheduled departure and arrival timings in order to document the specifics of the journeys taken, the traffic situation, etc. Flight information, such as the place of origin, the destination, the date of the flight, the scheduled time of departure and arrival, etc.  Information about weather stations, such as station ID and associated AirportID, ground height, etc. Additionally offered are hourly aviation meteorological conditions data for 2 years, etc. Flight data's origin and destination information can be mapped to other datasets' AirportIDs.

Data consists of flights data, weather information along with stations information from the year 2014 and 2015. The aggregated/consolidated train dataset for model building and tuning the model is used and then applied the model on test data for obtaining the predictions.

The datasets used are cited below for the analysis:
1. Flights Data:
  > “Train.csv” & 	“Test.csv”
  > These files consist of the Flight details  of each ID, like ID, Origina, destination, date, timestamps etc.
  >	Target attribute “FlightDelayStatus”  is derived from the delay based on ActualArrivalTimeStamp given in Train.csv, where as Test.csv doesn’t have this 
    attribute as a “FlightDelayStatus”  is predicted.
  > If the delay is more than  15 minutes then FlightDelayStatus will be “1” else “2”

2.  AllStationsData_PHD.txt :
  > This flie gives the link of ""WeatherStationID""  & ""AirportID""  
  > This has the attributes viz.,  Latitude, Longitude, TimeZone etc

3.  Weather information:
  >	Folder “weatherdatatoconsider” has sub-folders 2004 and 2005    
  >	These files consist of the details about aviation weather during the 2004 and 2005  
  > Each folder has month  wise .txt files in which hourly data is there –  a set f aviation weather hourly .txt files  and another se of  precipitation related 
    weather .txt files

4. Attributes Details: “AttributeInformation.docx
  > This has the details of attributes for the 	datasets 	cited above (1 to  3)

Note: For analysis all the datasets cited above (1) to (3) are consolidate/aggregated.


