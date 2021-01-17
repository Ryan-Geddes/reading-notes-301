
# Oauth

## Write the following steps in the correct order:

- Register your application to get a client_id and client_secret
- Redirect to a third party authentication endpoint
- Ask the client if they want to sign in via a third party
- Receive authorization code
- Make a request to the access token endpoint
- Receive access token
- Make a request to a third-party API endpoint


## What can you do with an authorization code?
Make a request to the access token endpoint

## What can you do with an access token?
access certain information from an API

## What’s a benefit of using OAuth instead of your own basic authentication?
Easier to implement and provides stronger authentication. Protects user data by providing access to the data without revealing the user’s identity or credentials. Third-party services can make requests on behalf of a user without accessing passwords and other sensitive information.

# Vocabulary Terms
- **Client ID**   public identifier for apps
- **Client Secret**   secret known only to the application and the authorization server
- **Authentication Endpoint** the endpoint on the authorization server where the resource owner logs in, and grants authorization to the client application
- **Access Token Endpoint**  where apps make a request to get an access token for a user.
- **API Endpoint** a specified location from which API's can access the resources they need to carry out their function.
- **Authorization Code** unique code that the user is given after logging in via a third party service.
- **Access Token**  token given once user is authorized. Contains the security credentials for a login session and identifies the user, the user’s groups, the user’s privileges, and, in some cases, a particular application





How to insert cursor at beginning of every line:

Press CTRL + A to select all of the text.
Press SHIFT + ALT + I to insert multiple cursors at the end of each line.
Press Home twice to jump to the start of every line.
