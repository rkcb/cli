
# Open Postgresql terminal as user postgre

sudo -u postgres psql postgres

# Change securely the password of a username

\password username

# Location of config file 

/var/lib/postgres/data/pg_hba.conf



## Misc

- login to database:
        * psql -d mydb -U myuser

- create a new user:
        * su - postgres
        * createuser --interactive --pwprompt

- create a new database:
        * createdb -O ownerOfDatabase mydatabaseName​