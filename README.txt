Updated 1 dec 2016

How to run:

in Ubuntu

virtualenv -p /usr/bin/python3 venv [Python 3.5]
source venv/bin/activate
pip install Django==1.8

[edit rhymes/settings.py and change location of db file]

[to change user password] (doesn't seem to work)

python manage.py shell

from django.contrib.auth.models import User
u = User.objects.all()[0]
u.set_password("new password")

URLs
rhymes/build
rhymes/match   ex. use pinyin: rhymes/match/i-ao 
rhymes/search
