Install development environment
-------------------------------


Open up Terminal and do the following

1. Set up your virtualenv

	~> virtualenv -p --no-site-packages Open_env
	~/Open_env> source bin/activate

2. Clone Repository

    	~/Open_env> git clone git@github.com:roggrat/OpenSMS.git

3. Install dependencies 

    	~/Open_env> cd HarukaSMS
    	~/Open_env/OpenSMS> pip install -r requirements.txt

4. Start a new Terminal Session. (This is to ensure that step 6 works)

6. Create the database

    	~/Open_env/OpenSMS> python manage.py syncdb

7. Run the development webserver
 
	~/Open_env/OpenSMS> python manage.py runserver 0.0.0.0:80 &

8. Run the GSM router using Kannel

        service kannel start 

		
		
