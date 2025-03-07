# CapstoneExploration/flask

A subdirectory to explore the use of [flask](https://flask.palletsprojects.com/en/2.0.x/) for our project's frontend.

## To Do List
- Explore [quickstart guide](https://flask.palletsprojects.com/en/2.0.x/quickstart/) in-depth
- Configure HTML rendering templates with jinja, as described in the [quickstart guide](https://flask.palletsprojects.com/en/2.0.x/quickstart/)
- Add bootstrap for aesthetic upgrades
- Load an iframe basemap from an external source (Google/OpenStreetMap)
- Load data layers from external APIs (NOAA/NASA)

## Activity Log

#### 14 February 2022
- Updated form to look more like mockups
- Added a wind direction slider
- Updates to overall page format
- Selectable layers

#### 6 February 2022
- Changed most of the inputs page to look like mockups
- Added sliders and impacts page button
- Added some slight css to format page
- No radio buttons added yet, impacts page will need updates
- Not sure if the baseline section should have its own submission button? Or if clicking the radio button to left will automatically pull data, and then eye button will display that data? Need a way for that button to submit without hitting the run option


#### 31 January 2022
- Added example user form for inputting parameters
- Created prototype page for testing data and such that is not in the nav bar
- Added handler for the form


#### 22 January 2022
- Restructured flask app files to comply with [standard layout](https://flask.palletsprojects.com/en/2.0.x/tutorial/layout/)
  - `wsgi.py` boots the app
  - `__init__.py` initializes the app
  - `routes.py` defines url pathways for the app
  - Files in `static/` contain images, data, style files, etc. not modified by the app
  - Files in `templates/` render HTML views
  - Files in `tests/` serve to test functionalities of the app
- Implemented bootstrap CSS styling, navbar, and footer
- Implemented jinja base HTML template in `application/templates/base.html`
- Added basic test in `tests/test_init.py`
  - To run a test in PyCharm, right click on the `flask` subdirectory and select "Mark Directory as > Sources Root", then click the play button within each test file. For more, see [this PyCharm post](https://www.jetbrains.com/help/pycharm/performing-tests.html).
  - To run all tests in the `flask/test` subdirectory from command line, set your working directory to `CapstoneExploration/flask` then run `python -m unittest`. This will discover all tests within `flask/test` and run them at once. For more, see [this StackOverflow post](https://stackoverflow.com/a/43733357).


#### 20 January 2022
- Created skeleton website, without any styling yet
  - Added navigation bar to each page that we expect to have, along with the corresponding pages
  - Added filler text to each page about what we plan to implement

#### 17 January 2022
- Added demo flask app in `app.py`
- Run this demo by:
  - Opening a powershell/cmd/terminal in `CapstoneExploration/flask`, then
  - Setting environment variables with `export FLASK_APP="wsgi"` in bash or `$env:FLASK_APP="wsgi"` command in Powershell 
  - Running `flask run`, and
  - Clicking on the localhost link returned by flask to view the webpage.
  