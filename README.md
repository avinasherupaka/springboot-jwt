# springboot-jwt

This Project uses JWT to secure the REST endpoints.

The Following are the REST end points available in the example.

#Getting Token:
_http://localhost:8080/token_ - Generates the JWT token based on the JSON sent. 
    1. **Operation** POST:
    2. **accepts - JSON(application/json)**: { "username": "name", "id": 123, "role": "admin"}

#Testing AUTH:
_http://localhost:8080/rest/hello_ - Requires a JWT Token and returns a resource 
    1. **Header key** - "Bearer"
    2. **value** - "Token <JWT_Token>"