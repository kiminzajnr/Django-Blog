#Setup

in a python virtual environment, run:\
-: $ pip install -r requirements.txt\
-: $ python3 manage.py makemigrations blog\
-: $ python3 manage.py migrate blog\
-: $ python3 manage.py createsuperuser == To create user that you'll use to log in\
Note: To activate the virtual environment cd into the directory then type $ source myvenv/bin/activate\


#Running the application\

$ python manage.py runserver\
Your blog is now ready\


#Test

python3 manage.py test\


#Login and out

-: Click <Log in> - you will be directed to Admin page\
-: As <Log in> credentials, use those created for superuser in Setup\
-: Click on <Log out> to log out\


#Blog entry

Log in and click on the <+> button , enter the title and text and finally save. While logged in, you'll enjoy all superuser privilleges including deleting a post or saving to draft\


#Deploying your blog to pythonanywhere.com

Note: To deploy to pythonanywhere, you should push your code to github\

Create your pythonanywhere beginner account at www.pythonanywhere.com\
While at your dashboard, navigate to account and click create a new API token\
Go back to pythonanywhere dashboard then choose start a "Bash" console\
At the pythonanywhere commandlile type this command: $ pip3.6 install -- user pythonanywhere\
Then type this command $ pa_autoconfigure_django.py --python=3.6 https://github.com/<your-github-username>/Django-Blog.git\
Also type this command to create an admin panel: You can put different credentials from those you used in the Setup if you want $ python manage.py createsuperuser\
To check your site click pythonanywhere "Web" page to get a link to it:)\


