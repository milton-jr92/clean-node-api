# Login

> ## Use case

1. ✅ Receives a **POST** request in route **/api/login**
2. ✅ Validates required data **email** and **password**
3. ✅ Validates that the field **email** is a valid e-mail
4. ✅ **Searches** the user by email and password provided
5. ✅ Creates an access **token** from user's ID
6. ✅ **Updates** user's data with the created access token
7. ✅ Returns **200** with access token and the user's name

> ## Exceptions

1. ✅ Returns error **404** if the API does not exist
2. ✅ Returns error **400** if **email** or **password** are not provided by client
3. ✅ Returns error **400** if **email** is an invalid e-email
4. ✅ Returns error **401** if the user is not found with the data provided
5. ✅ Returns error **500** if it fails to create the access token
6. ✅ Returns error **500** if it fails to update the user with the access token
