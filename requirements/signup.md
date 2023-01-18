# Sign Up

> ## Use case

1. ✅ Receives a **POST** request in route **/api/signup**
2. ✅ Validates required data **name**, **email**, **password** and **passwordConfirmation**
3. ✅ Validates that **password** and **passwordConfirmation** are equals
4. ✅ Validates that the field **email** is a valid e-mail
5. ✅ **Validates** if the user already exists given the email provided
6. ✅ Generates a password **encrypted** (this password can't be decrypted)
7. ✅ **Creates** the user account with the given data, **replacing** the password with encrypted password
8. ✅ Generates an access **token** from user's ID
9. ✅ **Updates** user's data with the created access token
10. ✅ Returns **200** with access token

> ## Exceptions

1. ✅ Returns error **404** if the API does not exist
2. ✅ Returns error **400** if **name**, **email**, **password** or **passwordConfirmation** are not provided by client
3. ✅ Returns error **400** if **password** and **passwordConfirmation** are not equals
4. ✅ Returns error **400** if **email** is an invalid e-email
5. ✅ Returns error **403** if the provided **email** already exists 
6. ✅ Returns error **500** if it fails to create an encrypted password
7. ✅ Returns error **500** if it fails to create the user account
8. ✅ Returns error **500** if it fails to create the access token
9. ✅ Returns error **500** if it fails to update the user with the access token
