## Outcome Based Course

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


## Software Carpentary Make

Make is a tool which can run commands to read files, process these files in some way, and write out the processed files. For example, in software development, Make is used to compile source code into executable programs or libraries, but Make can also be used to:

run analysis scripts on raw data files to get data files that summarize the raw data;

run visualization scripts on data files to produce plots; 

and to parse and combine text files and plots to create papers.

Introduction 

To make my results easier to reproduce

Automatic variables

To write a simple Makefile

Dependencies on data and code

To write a Makefile to update things when my scripts have changed rather than my input files

Pattern Rules :

To define rules to operate on similar files

Variables:

To eliminate redundancy in my Makefiles

Functions

To eliminate redundancy in my Makefiles

Self Documenting makefiles

To document a Makefile

Conclusion

The advantages and disadvantages of using tools like Make


## Block with github pages

To start a jekyll blog on github pages :

1. Create a new repository on github

2. Install jekyll

ruby -v

gem -v

sudo gem install jekyll

jekyll -v

3. Create a jekyll site

jekyll new myjekyllblog

jekyll serve --watch


4. Change the configurations

Your Jekyll blog’s configurations reside in the _config.yml file. When you install Jekyll it comes with a default config. Open the file in a code editor and change the values.

5. Add Blog Posts

year-month-date-{slug}.md

6. Push the site live

git init

git add .

git commit -m "Initial commit"

git remote add origin https://github.com/myjekyllblog/myjekyllblog.github.io

git push origin master

## Shell Script tutorial

This tutorial is written to help people understand some of the basics of shell script programming (aka shell scripting), and hopefully to introduce some of the possibilities of simple but powerful programming available. 

To start the project , use any text editor and save it as .sh file.

#!/bin/bash

echo "Hello World!"

To run

cd src/

$ chmod +x ./hello_world.sh

$ ./hello_world.sh

Variable declaration

intVar="233"

To run

echo $intVar

Basic Operations

a=233

b=666

val1=`expr $a + $b`

echo "Total value: $val1"
## Django Installation 

Step 1 — Install Python and pip

sudo apt-get update && sudo apt-get -y upgrade

sudo apt-get install python3

python3 -V

sudo apt-get install -y python3-pip

pip3 -V

Step 2 — Install virtualenv

pip3 install virtualenv

virtualenv --version

Step 3 — Install Django

mkdir django-apps

cd django-apps

virtualenv env

. env/bin/activate

Once it’s activated the prefix is changed to (env),

(env) varsha@varsha-X556UQK:$ pip install django

(env) varsha@varsha-X556UQK:$ django-admin --version



## Ubuntu Installation

_Installing Linux using USB stick :_

Step 1) Download the .iso or the OS files on your computer

Step 2) Download free software like 'Universal USB installer to make a bootable USB stick.

Step 3) Select an Ubuntu Distribution form the dropdown to put on your USB

Select your Ubuntu iso file download in step 1.

Select the drive letter of USB to install Ubuntu and Press create button.

Step 4) Click YES to Install Ubuntu in USB.

Step 5) After everything has been installed and configured, a small window will appear Congratulations! You now have Ubuntu on a USB stick, bootable and ready to go.







