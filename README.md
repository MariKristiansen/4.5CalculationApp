In this task, you need to create the calculator application.

Create the REST API with three endpoints:
- GET /sum/:number1/:number2 – returns the sum of two numbers provided  in route parameters.
- POST /favNumber – sets the favourite number (if currently there is one, it is overridden). 
    Example of request body for POST:
        {
        "number":1
        }
- DELETE /favNumber – deletes favourite number (set it to default value).

Favourite number can be stored in a SQL database or JSON file.
Favourite number is 0 by default. It is added to each result, so after setting it with POST method to 3, the GET sum/2/5 will return 10 (2+5+3).
Next, create unit and integration tests for the application.