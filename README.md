# The quiz application

* a Flask starter project for quizzes
* available live at https://johnreeves.pythonanywhere.com/

### Code directories
```code
Source code:             /home/johnreeves/quiz
Working directory:       /home/johnreeves/quiz
WSGI configuration file: /var/www/johnreeves_pythonanywhere_com_wsgi.py
Python version:          3.10
```

### WSGI configuration
```code
# This file contains the WSGI configuration required to serve up your
# web application at http://<your-username>.pythonanywhere.com/
# It works by setting the variable 'application' to a WSGI handler of some
# description.
#
# The below has been auto-generated for your Flask project

import sys

# add your project directory to the sys.path
project_home = '/home/johnreeves/quiz'
if project_home not in sys.path:
    sys.path = [project_home] + sys.path

# import flask app but need to call it "application" for WSGI to work
from quiz import app as application  # noqa
```


### Static files:
```code
Files that aren't dynamically generated by your code, like CSS, JavaScript or uploaded files, can be served much faster straight off the disk if you specify them here. You need to Reload your web app to activate any changes you make to the mappings below.

URL	        Directory
/static/         /home/johnreeves/quizzes/static	 
/quizzes/        /home/johnreeves/quizzes/quizzes	 
/data/           /home/johnreeves/quizzes/data	 
/templates/      /home/johnreeves/quizzes/templates	 
```

### Folder structure
```
project/
│
├── static/
│   ├── style.css                 # CSS for styling
│   └── script.js                 # JavaScript for quiz interactivity
│
├── templates/
│   └── index.html                # HTML file to be rendered by Flask
│
├── quizzes/
│   ├── quiz1.json                # Example JSON file with quiz questions
│   └── science_quiz.json
│
├── data/
│   ├── quiz1_responses.json      # Example JSON file with quiz responses
│   └── science_quiz_responses.json
│
├── high_scores.json              # JSON file of high scores for each quiz
└── quiz.py                       # Flask server script
```
