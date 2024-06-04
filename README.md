# Weather Data - Easley/Greenville SC
Historical daily weather data for Easley and Greenville, SC.

Includes: 
- SQL for creating the WEATHER_DATA table in Oracle
- Oracle Datamining workflow for generating charts for total rainfall by year

## Response weather data elements
The following are the list of properties in a day or hourly data object:

- **cloudcover** – how much of the sky is covered in cloud ranging from 0-100%.
- **conditions** – textual representation of the weather conditions.
- **description** – longer text descriptions suitable for displaying in weather displays. The descriptions combine the main features of the weather for the day such as precipitation or amount of cloud cover. Daily descriptions are provided for historical and forecast days. When the timeline request includes the model forecast period, a seven day outlook description is provided at the root response level.
- **datetime** – ISO 8601 formatted date, time or datetime value indicating the date and time of the weather data in the local time zone of the requested location.
- **dew** – dew point temperature.
- **feelslike** – what the temperature feels like accounting for heat index or wind chill. Daily values are average values (mean) for the day.
- **feelslikemax** – maximum feels like temperature at the location.
- **feelslikemin** – minimum feels like temperature at the location.
- **humidity** – relative humidity in %.
- **icon** – a fixed, machine readable summary that can be used to display an icon.
- **moonphase** –  represents the fractional portion through the current moon lunation cycle ranging from 0 (the new moon) to 0.5 (the full moon) and back to 1 (the next new moon).
- **precip** – the amount of liquid precipitation that fell or is predicted to fall in the period. This includes the liquid-equivalent amount of any frozen precipitation such as snow or ice.
- **precipcover** – the proportion of hours where there was non-zero precipitation/
- **preciptype** – an array indicating the type(s) of precipitation expected or tha occurred. Possible values include rain, snow, freezingrain and ice.
- **sealevelpressure** – the sea level atmospheric or barometric pressure in millibars (or hectopascals).
- **source** –  the type of weather data used for this weather object. – Values include historical observation (“obs”), forecast (“fcst”), historical forecast (“histfcst”) or statistical forecast (“stats”). If multiple types are used in the same day, “comb” is used. Today a combination of historical observations and forecast data.
- **sunrise** – The formatted time of the sunrise (For example “2022-05-23T05:50:40”).
- **sunset** – The formatted time of the sunset (For example “2022-05-23T20:22:29”).
- **temp** – temperature at the location. Daily values are average values (mean) for the day.
- **tempmax** – maximum temperature at the location.
- **tempmin** – minimum temperature at the location.
- **uvindex** – a value between 0 and 10 indicating the level of ultra violet (UV) exposure for that hour or day. 10 represents high level of exposure, and 0 represents no exposure. The UV index is calculated based on amount of short wave solar radiation which in turn is a level the cloudiness, type of cloud, time of day, time of year and location altitude. Daily values represent the maximum value of the hourly values.
- **visibility** – distance at which distant objects are visible.
- **winddir** – direction from which the wind is blowing.
- **windgust** – instantaneous wind speed at a location – May be empty if it is not significantly higher than the wind speed. Daily values are the maximum hourly value for the day.
- **windspeed** – the sustained wind speed measured as the average windspeed that occurs during the preceding one to two minutes. Daily values are the maximum hourly value for the day.
- **windspeedmax** – maximum wind speed over the day.
- **windspeedmean** – average (mean) wind speed over the day.
- **windspeedmin** – minimum wind speed over the day.
- **solarradiation** – (W/m2) the solar radiation power at the instantaneous moment of the observation (or forecast prediction).
- **solarenergy** – (MJ /m2 ) indicates the total energy from the sun that builds up over an hour or day.
- **severerisk**  – a value between 0 and 100 representing the risk of convective storms (e.g. thunderstorms, hail and tornadoes). Severe risk is a scaled measure that combines a variety of other fields such as the convective available potential energy (CAPE) and convective inhibition (CIN), predicted rain and wind. Typically, a severe risk value less than 30 indicates a low risk, between 30 and 70 a moderate risk and above 70 a high risk.

Data source is https://www.visualcrossing.com/weather/weather-data-services
