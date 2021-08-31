# python-app-with-electron-gui
Use HTML, JavaScript and CSS to make highly customized, cross platfrom desktop apps which use native Python backends.

## General Dependenices
  * Python
  * NodeJS
  * electron.js
  * python-shell
 
## Specific Dependencies
  * weather module:
    * requests
    * beautifulsoup4
   
  * object detection module
    * Flask
    * tensorflow
    * keras
    
    ## Usage
    * Clone the repo, and then
	```sh
	$ cd electron-app-with-python-gui
	$ pip install -r requirements.txt
	$ npm install
	$ npm start
	```
    * If you want to use the object detection module, make sure the flask server [object_detection.py] is up and running before starting the GUI.
	```sh
	$ cd engine
	$ python object_detection.py
	```

## Note:

weather_engine.py uses web-scraping to pull data off the internet, from a particular website. If this site happens to be modified
or changed in the future, the code *might* break. However, this can be fixed by analyzing the new layout of the site and adjusting
the python code accordingly.
