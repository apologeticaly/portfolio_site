Q: (5 Points) How is this project structure different than a Flask (or Node) application? What role are the urls.py and views.py files responsible for?

A: The url.py and views.py files serve almost like a dictionary to direct the routes generally based on the passed parameters (in this case the url), and then conditionaly serve a webpage. Flask and Node (usualy) need a canonical link that is unchanging, which is hardcoded.


Q: (5 Points) Why do we use 2 separate urls.py files? How do they interact?

A: The global (root) urls.py file serves the route for the entire website, while the urls.py in the app folder serve the routes for that particular app (i.e. messages/).


Q: (5 Points) When is it desirable to split our code over multiple apps? Why would we want to do so?

A: For large chunks of the website that don't need a url change. For example, and admin page, inwhich all the functionaly resides within the admin/ rout. Another example would be a editor/ route for at a web-based IDE. There is no need for the url to chagne while using, so all the functionality can be contained to that app.