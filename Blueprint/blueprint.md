FORMAT: 1A
HOST: http://afdemocarsapi.azurewebsites.net/api

# Cars API
API to handle all company cars.

## Cars [/cars]
### List all company cars [GET]
+ Response 200 (application/json)

        [{
          "Id": 1, "Make": "Volvo", "Model": "XC60", "Year": 2015
        }, {
          "Id": 2, "Make": "Renault", "Model": "Megane", "Year": 2012
        }]

+ Parameters
    + s (optional, string, `Volvo`) ... A search string.

## Car [/cars/{id}]

### Get specific car [GET]

+ Response 201 (application/json)

        {
          "Id": 1, "Make": "Volvo", "Model": "XC60", "Year": 2015
        }
        
+ Parameters
    + id (required, number, `1`) ... The id of the car to get.
