# Conversation With API Builders

* Return 200 when it is all good
* Return 400 when the request payload is not valid
* Return 422 when the input data is not valid
* Return 401 when user is not authenticated
* Return 403 when user is not authorized
* Return 404 when record is not found
* Return 500 when an error is encountered
* No need to have success key in response
* Do not use redirect in API
* Response should be valid JSON even when things go wrong

from https://conversation.bigbinary.com/