**Pizza Maker**

This is an express app tied to a single-component Angular application.

**Setup and installation:**

1. From the project root, `npm install` to install the needed dependencies for the express server.
2. `nodemon` from the terminal, and you are good to go! (Make sure `mongod` is up and running as well!)
3. If you wish to modify the angular source code:
	4. `cd public` to get into the angular directory
	5. `npm install` to install angular and its dependencies
	6. `ng build -w` to rebuild your angular app whenever changes are made.

**Important Files**

* server.js
	* No more ejs!
	* the static root is declared as the 'dist' directory created by the angular cli `ng build` command
	* 	body parser is configured to accept json instead of urlencoded

* server/controllers/pizzas.js
	* The responses are all in json format instead of rendering a template from ejs