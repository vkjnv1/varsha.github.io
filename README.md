## To provide extra space to ubuntu

03 march 2020

- Install gparted in ubuntu :

sudo apt list --installed | grep gparted

sudo apt-cache search gparted

sudo apt-get install gparted

sudo gparted &

and then follow the steps mentioned in the link :

[https://www.youtube.com/watch?v=5y47WD_RRFc]

## Outcome Based Course




## Outcome Based Course

24 feb 2020 - 27 feb 2020

_Steps for installation of OutcomeBasedCourse:_

-> Clone the repository OutcomeBasedCourse.

 git clone https://github.com/GreatDevelopers/OutcomeBasedCourse
 
-> Create a database for OutcomeBasedCourse.

  mysql -u root -p -e "create database outcomebasedcourse;"
  
-> Edit settings.py file in OutcomeBasedCourse/ directory. Things to be edited are:

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
  
-> Goto the project directory and run the following commands:

 python3 manage.py makemigrations
 
 python3 manage.py migrate
 
 python3 manage.py runserver 127.0.0.1:8090
 
Open "http://127.0.0.1:8090" in your browser.

[https://github.com/GreatDevelopers/OutcomeBasedCourse]


## Software Carpentary Make
22 feb 2020 - 23 feb 2020

_Make is a tool which can run commands to read files, process these files in some way, and write out the processed files. For example, in software development, Make is used to compile source code into executable programs or libraries, but Make can also be used to:_

1. run analysis scripts on raw data files to get data files that summarize the raw data.

2. run visualization scripts on data files to produce plots.

3.  parse and combine text files and plots to create papers.

- Introduction :

To make my results easier to reproduce

- Automatic variables

To write a simple Makefile

- Dependencies on data and code

To write a Makefile to update things when my scripts have changed rather than my input files

- Pattern Rules :

To define rules to operate on similar files

- Variables:

To eliminate redundancy in my Makefiles

- Functions

To eliminate redundancy in my Makefiles

- Self Documenting makefiles

To document a Makefile


## Block with github pages

21 feb 2020

_To start a jekyll blog on github pages :_

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

_Your Jekyll blog’s configurations reside in the _config.yml file. When you install Jekyll it comes with a default config. Open the file in a code editor and change the values._

5. Add Blog Posts

year-month-date-{slug}.md

6. Push the site live

git init

git add .

git commit -m "Initial commit"

git remote add origin https://github.com/myjekyllblog/myjekyllblog.github.io

git push origin master

## Shell Script tutorial

20 feb 2020

_This tutorial is written to help people understand some of the basics of shell script programming (aka shell scripting), and hopefully to introduce some of the possibilities of simple but powerful programming available._ 

- To start the project , use any text editor and save it as .sh file.

#!/bin/bash

echo "Hello World!"

- To run

cd src/

$ chmod +x ./hello_world.sh

$ ./hello_world.sh

- Variable declaration :

intVar="233"

- To run

echo $intVar

- Basic Operations :

a=233

b=666

val1=`expr $a + $b`

echo "Total value: $val1"

- Relational Operators :

if [ $a -eq $b ]
then
    echo "a is equal to b"
else
    echo "a is not equal to b"


String Operators :
string1="Harry"
string2="Potter"

string3=$string1" "$string2 # string concatenation

echo $string3       # print string3

echo ${#string3}    # print length of string3

echo ${string3:2:5} # print slice of string3

- Array :

array=(1 2 3 4 5)

array2=(aa bb cc mm ee)

val=${array[2]}

echo $val

val=${array2[3]}

echo $val

length=${#array[*]}

echo $length

- Functions :

func(){
    intVar1=3
    intVar2=5
    return $(($intVar1+$intVar2))
}

- Call the function
func
result=$?
echo $result


## My_Project

16 feb 2020 - 17 feb 2020

It is a website using django framework that can remove unnecessary Punctuation marks, can change the sentence to UPPERCASE format ,can remove new lines and extraspace . 

These are done by four different functions :-

1. capfirst()

2. newlineremove()

3. spaceremove()

4. charcount()

 To start a project -
 
 django-admin startproject my_project

To run the project -

Go into project directory and run the command after completing the project -

python3 manage.py runserver

## Django Installation 

15 feb 2020

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

14 feb 2020

_Installing Linux using USB stick :_

Step 1) Download the .iso or the OS files on your computer

Step 2) Download free software like 'Universal USB installer to make a bootable USB stick.

Step 3) Select an Ubuntu Distribution form the dropdown to put on your USB

Select your Ubuntu iso file download in step 1.

Select the drive letter of USB to install Ubuntu and Press create button.

Step 4) Click YES to Install Ubuntu in USB.

Step 5) After everything has been installed and configured, a small window will appear Congratulations! You now have Ubuntu on a USB stick, bootable and ready to go.







