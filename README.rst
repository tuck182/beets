This is beets v1.3.6 with postgresql 8.4 support using psycopg2. It has been hacked and tested by a python novice in a few hours.
Create a database-user for your beets database and configure the database server in db.py under "def _connection(self):"
 else:
     # Make a new connection.
     conn = psycopg2.extras.RealDictConnection("host=localhost port=5432 dbname=beetsprod user=beetsprod password=beetsprod",
     
then run beets as usual. Enjoy!
