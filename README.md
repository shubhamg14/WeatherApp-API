# WeatherApp-API
Restful API for weather data

This API is created to read a CSV file which contains weather data for a city for past 5 years and make modifications to data using GET, POST, DELETE API requests.

**API also holds following functionalities** 

1. **Forecast for Existing and future dates.**
   It basically calculates the running average for past 365 days for any given date and then ouputs the forecast for next 7 days and if date for which forecast is requested is already present in the CSV file, then data for that date is outputted from CSV.
    
2. **Pull data from a third party API (Openweathermap.com).**
    Created an account on Openweathermap.com and generated an API key.
    Used API key to access live 5 Day forecast API on Openweather.com and pull that data as part of our /openweather API call. 

### Following end points and funtionality has been added to the API.

   ![alt text](https://github.com/shubhamg14/WeatherApp-API/blob/master/images/endpoint-descriptions.PNG)

### Responses from API are in the following format

   ![alt text](https://github.com/shubhamg14/WeatherApp-API/blob/master/images/api-responses.PNG)


## Following packages are required to run this code base:
1. Python (sudo apt install python)
2. pip 19.0.3 (sudo apt install python-pip)
3. Flask 1.0.2 (sudo pip install flask)
4. requests 2.21.0 (sudo pip install requests)
5. POSTMAN (Can be downloaded from getpostman.com)

## Running code 
        1. Create a project folder in your local file system and copy the following files into it:
                flaskapp_api
                dailyweather.csv
           
         2. Go to linux shell and install all dependent libraries mentioned in previous section using the commands given with them in               the same order.
         
         3. Go to your project folder in command prompt and then run command "python3 flaskapp_api.py"
         
         4. Your application will go live and then you can validate all endpoints using POSTMAN or any other api validating tools.

