# SAS-19
STEP 1: Installation: We will require two package to setup your environment. virtualenv for a user to create multiple Python environments side-by-side. Thereby, it can avoid compatibility issues between the different versions of the libraries and the next will be Flask itself.

virtualenv pip install virtualenv

Flask pip install Flask

After completing the installation of the package, let’s get our hands on the code.

from flask import Flask app = Flask(name) @app.route('/') def hello_world(): return 'Hello World' if name == 'main': app.run()

STEP 2: Save it with a file name myflask1.py and then run the script we will be getting an output.

STEP 3: Then go to the url given there you will seeing your first webpage displaying hello world there on your local server. Go to the url http://127.0.0.1:5000/

STEP 4: Digging further into the context, the route() decorator in Flask is used to bind URL to a function. Now to extend this functionality our small web app is also equipped with another method add_url_rule() which is a function of an application object is also available to bind a URL with a function as in the above example, route() is used.

Modify myflask1.py and add the following lines of code then save it. Don’t forget to run again the script.

from flask import Flask app = Flask(name) @app.route('/hello/') def hello_name(name): return 'Hello %s!' % name if name == 'main': app.run()

STEP 5: Go to the url http://127.0.0.1:5000/hello/ Replace with your name.

Example: http://127.0.0.1:5000/hello/Juan

STEP 6:Save your file for checking.

Go to your cmd and run the myflask2.py.

After the development server starts running, open login.html in your browser.

Enter your name in the text field and click the submit button.
