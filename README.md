# vetro-app
Run npm start then go to http://localhost:3000

# okta
I will be using Okta as an API service for managing user identities in order to handle the user registration, login, logout and CRUD.

Base URIs: http://localhost:3000/
Login redirect URIs: https://localhost:3000/authorization-code/callback

Express.js set up. 

# node modules
Please make sure you extract the node_modules.zip folder to the main file. Files are over a 200.

Installed the following modules for setting up my database:
npm install sqlite3@4.0.4 sequelize@4.42.0 epilogue@0.7.1 --save 
node-pre-gyp install --fallback-to-build

# adding authentication in Express
Okta middleware takes care of the login using the app.use(oidc.router). 
Now, we can visit http://localhost:3000/home to login which directs us to the Okta login page.

# admin page
Set up the /admin in the application as the defaultRedirect URL in the ExpressOIDC setup to see the admin page.

# setting up our SQLite database in Express.js
Using SQLite as our database for storage using Sequelize and created the REST endpoints using Epilogue. Also, I added an authentication check to all CRUD routes using the code in PostResource.all.auth section. 

# public folder created
admin.html 
admin.js 
home.html 
home.js 

# login and logout button
Load the React JavaScript and bootstrap CSS files for the home page and admin.js will render the navigation menu with the Logout button. It will also render the Add New Post button.

# home page
Now, if you go to http://localhost:3000/home, run npm start and log in, you should able to add new posts, update, and delete existing posts!
