# Classification for Fligth Data : Delayed or Not
My study of classifiying whether a flight is delayed by looking at the given flight dataset.

## Given Dataset Features
<b>FL_DATE</b>: Flight Date (yyyymmdd)<br>
<b>OP_UNIQUE_CARRIER</b>: Unique Carrier Code<br>
<b>OP_CARRIER_FL_NUM</b>: Flight Number<br>
<b>ORIGIN</b>: Origin Airport Code<br>
<b>DEST</b>: Destination Airport Code<br>
<b>CRS_DEP_TIME</b>: CRS Departure Time (local time :  hhmm)<br>
<b>DEP_TIME</b>: Actual Departure Time (local time :  hhmm)<br>
<b>DEP_DELAY</b>: Difference in minutes between scheduled and actual departure time. Early departures show negative numbers.<br>
<b>CRS_ARR_TIME</b>: CRS Arrival Time (local time :  hhmm)<br>
<b>ARR_TIME</b>: Actual Arrival Time (local time :  hhmm)<br>
<b>ARR_DELAY</b>: Difference in minutes between scheduled and actual arrival time. Early arrivals show negative numbers.<br>
<b>CANCELLED</b>: Cancelled Flight Indicator (1=Yes)<br>
<b>CANCELLATION_CODE</b>: Specifies The Reason For Cancellation<br>
<b>CRS_ELAPSED_TIME</b>: CRS Elapsed Time of Flight, in Minutes<br>
<b>ACTUAL_ELAPSED_TIME</b>: Elapsed Time of Flight, in Minutes<br>
<b>AIR_TIME</b>: Flight Time, in Minutes<br>
<b>DISTANCE</b>: Distance between airports (miles)<br>
<b>CARRIER_DELAY</b>: Carrier Delay, in Minutes<br>
<b>WEATHER_DELAY</b>: Weather Delay, in Minutes<br>
<b>NAS_DELAY</b>: National Air System Delay, in Minutes<br>
<b>SECURITY_DELAY</b>: Security Delay, in Minutes<br>
<b>LATE_AIRCRAFT_DELAY</b>: Late Aircraft Delay, in Minutes<br>

## Things to note:
1. Data consists of 14 months, where 12 months (07.2018 - 06.2019) are for training/validation and
2 months (07.2019 - 08.2019) for testing purposes.
2. DepDelay (in minutes) is your target variable.
3. From an operational perspective, flight is classified as delayed, when it is late 15 minutes or more.
4. Scheduled departure time of the flight is the last available moment for doing prediction.
5. For modeling/analysis use a subset of 8 carriers, which are the most common in the dataset.
6. Feel free to use any publicly available information/dataset for feature engineering.
7. Don’t forget about exploratory data analysis (at least 3 questions & answers).
