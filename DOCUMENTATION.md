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
                  "id": "e98e472f-7e4f-4b0e-a1f6-dfb43a283ca0",
                  "firstName": "John",
                  "lastName": "Smith",
                  "email": "johnsmith@example.com"
                  "phone number": 08055628562,
                  "address": "Lagos",
                  "Photo": "Base64"
                }
          ```
- POST /api/register: Create a new user

    - Description: Create a new user on the platform.
    
    - Request: User object with required fields (email, first_name, last_name).
        
        - Response:
            
        - Status Code: 201 (Created)

        - Response Body: User object of the created user

        - Example Response:
     
          ```
                {
                  "id": "e98e472f-7e4f-4b0e-a1f6-dfb43a283ca0",
                  "Photo": "Base64"
                  "email": "smith.mike@example.com",
                  "username": "mikesmith",
                  "password": "admin@123"
                }
          ```

- PUT /api/updateuser/:id: Update a user

    - Description: Update an existing user's information.

    - Request: User object with fields to update.
    
    - Response:
        
        - Status Code: 200 (OK)

        - Response Body: User object of the updated user
     
- DELETE /api/users/:id: Delete a user

    - Description: Delete a user from the platform.

    - Request: No request body required.

    - Response:
        
        - Status Code: 204 (No Content)
