Steps for installation of OutcomeBasedCourse:

Clone the repository OutcomeBasedCourse.

 git clone https://github.com/GreatDevelopers/OutcomeBasedCourse
Create a database for OutcomeBasedCourse.

  mysql -u root -p -e "create database outcomebasedcourse;"
Edit settings.py file in OutcomeBasedCourse/ directory. Things to be edited are:

 DATABASES = {
          "default":  {
                 "ENGINE": "django.db.backends.mysql",
                 "NAME": "Your database name"
                 "HOST": "Your MySQl server host",
                 "PORT": "Your MySQl server port",
                 "USER": "Your MySQL username",
                 "PASSWORD": "Your MySQl password",
          } 
  } 
Goto the project directory and run the following commands:

 python3 manage.py makemigrations
 python3 manage.py migrate
 python3 manage.py runserver 127.0.0.1:8090
Open "http://127.0.0.1:8090" in your browser.
