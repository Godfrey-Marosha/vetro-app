# vetro-app
Run npm start then go to http://localhost:3000

# okta
I will be using Okta as an API service for managing user identities in order to handle the user registration, login, logout and CRUD.

Base URIs: http://localhost:3000/
Login redirect URIs: https://localhost:3000/authorization-code/callback

Express.js set up. 

# node modules
Please make sure you extract the node_modules.zip folder to the main file. Files are over a 200.

# adding authentication in Express
Okta middleware takes care of the login using the app.use(oidc.router). 
Now, we can visit http://localhost:3000/home to login which directs us to the Okta login page.

# admin page
Set up the /admin in the application as the defaultRedirect URL in the ExpressOIDC setup to see the admin page.
