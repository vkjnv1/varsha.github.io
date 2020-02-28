Django Installation

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

