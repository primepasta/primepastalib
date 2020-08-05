# primepastalib
Makes the necessary changes to your django files and deploys them to heroku.

Usage:

```python
from primepastalib import herokuLogin, djangoDeploy

#projectName is the name of your django project, and appName is the name that you'd your heroku app to have.

#adds the required files and makes changes to the settings.py file, and deploys them to heroku. Make sure you're logged in. Heroku will choose a name for the app.

djangoDeploy('projectName')

#Does the same as above, except the name you pass will be used for the app.

djangoDeploy('projectName', 'appName')

#You can also login to heroku by running the following: (It is recommended that you log into the heroku CLI yourself.)

herokuLogin()
```
