# my-postgresql-cheatseet

## Installation

Step 1: Download the source code.

Download PostgreSQL-9.6.8 binaries from the official PostgreSQL site or Click Here to download the source code.

Step 2: Extract the tar archive

gunzip postgresql-9.6.8.tar.gz
tar xvf postgresql-9.6.8.tar

gunzip postgresql-9.6.8.tar.gz
tar xvf postgresql-9.6.8.tar
cd postgresql-9.6.8
./configure

All files will be installed under /usr/local/pgsql by default.

## Getting Started

`$  sudo su - postgres`
`$ psql`

## Service management commands:
```
sudo service postgresql stop
sudo service postgresql start
sudo service postgresql restart
```
## Quick Help
```
\q: Quit/Exit
\c __database__: Connect to a database
\d __table__: Show table definition including triggers
\d+ __table__: More detailed table definition including description and physical disk size
\l: List databases
\dy: List events
\df: List functions
\di: List indexes
\dn: List schemas
\dt *.*: List tables from all schemas (if *.* is omitted will only show SEARCH_PATH ones)
\dT+: List all data types
\dv: List views
\df+ __function__ : Show function SQL code.
\x: Pretty-format query results instead of the not-so-useful ASCII tables
\copy (SELECT * FROM __table_name__) TO 'file_path_and_name.csv' WITH CSV: Export a table as CSV
```
