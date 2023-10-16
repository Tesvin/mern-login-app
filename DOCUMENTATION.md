# Endpoint Documentation For Profile App API

## Resources

The resources provided by this API are listed as follows:

##### Users

This resource handles operations carried out on a User entity.

- GET /api/user/:username: Fetch user details

    - Description: Returns users details.

    - Response:

        - Status Code: 200 (OK)
     
        - Example Response:

          ```
                {
                  "firstName": "John",
                  "lastName": "Smith",
                  "age": 25
                }
          ```
