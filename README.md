# Getting the correct access token for App Services authentication
Testing App Service audiences with MSAL and Python

This demo has and Azure App Service with "easy auth" authentication turned on. 

Using MSAL with device code flow to attempt to get a token with the right audience for the app service to accept the request.

Still not quite right. If I use the Microsoft Graph audience of "User.Read", I get a token with an audience of Microsoft Graph and this gets rejected. I have also tried sending scopes of:
1. client_id
2. api://client_id
3. api://client_id/.default

The code is in a notebook, but ideally the REST requests needed would provide a better understanding.
