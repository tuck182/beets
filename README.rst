This is beets v1.3.6 with postgresql 8.4 support using psycopg2. It has been hacked in a few hours and tested with a big 
music library.

1. Create a database-user e.g. "beets" for your beets database "beets" and configure the server in db.py under "def _connection(self):"
...
     # Make a new connection.
     conn = psycopg2.extras.RealDictConnection("host=localhost port=5432 dbname=beets user=beets password=secret",

2. Run beets as usual. 

3. Write awesome PSQL queries and enjoy...
